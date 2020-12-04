---
title: Rozwiązywanie problemu z PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573722"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="5be6b-102">Rozwiązywanie problemu z PRT</span><span class="sxs-lookup"><span data-stu-id="5be6b-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="5be6b-103">W przypadku wszystkich urządzeń, które mogą dokończyć uwierzytelnianie, należy w pełni zarejestrować i w odpowiednim stanie i móc uzyskać podstawowy token odświeżania (PRT).</span><span class="sxs-lookup"><span data-stu-id="5be6b-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="5be6b-104">Proces rejestracji hybrydowej dołączania Azure AD wymaga, aby urządzenia były w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="5be6b-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="5be6b-105">Działa również w sieci VPN, ale istnieją pewne zastrzeżenia.</span><span class="sxs-lookup"><span data-stu-id="5be6b-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="5be6b-106">Przesłuchamy klientów potrzebujących pomocy w rozwiązywaniu problemów dotyczących procesu rejestracji hybrydowych funkcji dołączania usługi Azure AD w ramach sytuacji zdalnej.</span><span class="sxs-lookup"><span data-stu-id="5be6b-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="5be6b-107">Poniżej przedstawiono podział tego, co się dzieje w trakcie procesu rejestracji.</span><span class="sxs-lookup"><span data-stu-id="5be6b-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="5be6b-108">**Środowisko uwierzytelniania w chmurze (Korzystanie z synchronizacji skrótu hasła w usłudze Azure AD lub uwierzytelniania przekazujące)**</span><span class="sxs-lookup"><span data-stu-id="5be6b-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="5be6b-109">Ten przepływ rejestracji jest również nazywany "przyłączeniem do synchronizacji".</span><span class="sxs-lookup"><span data-stu-id="5be6b-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="5be6b-110">System Windows 10 odnajduje rekord punktu SCP po zalogowaniu się użytkownika do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="5be6b-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="5be6b-111">Urządzenie najpierw usiłuje pobrać informacje o dzierżawie ze strony klienta usługi SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="5be6b-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="5be6b-112">Aby uzyskać więcej informacji, zobacz ten [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="5be6b-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="5be6b-113">Jeśli to nie uda, urządzenie komunikuje się z lokalną usługą Active Directory (AD), aby uzyskać informacje o dzierżawie od punktu połączenia usługi (SCP).</span><span class="sxs-lookup"><span data-stu-id="5be6b-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="5be6b-114">Aby zweryfikować punkt SCP, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="5be6b-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="5be6b-115">Zalecamy włączenie punktu SCP w REKLAMie i korzystanie tylko z funkcji SCP po stronie klienta w celu wstępnego sprawdzania poprawności.</span><span class="sxs-lookup"><span data-stu-id="5be6b-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="5be6b-116">System Windows 10 próbuje komunikować się z usługą Azure AD w kontekście systemowym, aby uwierzytelnić się w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5be6b-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="5be6b-117">Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta system przy użyciu skryptu łączności urządzenia testowego.</span><span class="sxs-lookup"><span data-stu-id="5be6b-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="5be6b-118">System Windows 10 wygeneruje certyfikat z podpisem własnym i zapisuje go pod obiektem komputera w usłudze AD — lokalnie.</span><span class="sxs-lookup"><span data-stu-id="5be6b-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="5be6b-119">Wymaga to, aby kontroler domeny był oparty na linii.</span><span class="sxs-lookup"><span data-stu-id="5be6b-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="5be6b-120">Obiekt urządzenia z certyfikatem jest synchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5be6b-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="5be6b-121">Cykl synchronizacji jest domyślnie co 30 minut, ale zależy od konfiguracji usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5be6b-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="5be6b-122">Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="5be6b-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="5be6b-123">Na tym etapie powinno być możliwe wyświetlenie urządzenia subject w stanie "oczekujące" w obszarze Kaseta urządzenia usługi Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="5be6b-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="5be6b-124">Po następnym zalogowaniu się użytkownika do systemu Windows 10 rejestracja zostanie zakończona.</span><span class="sxs-lookup"><span data-stu-id="5be6b-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="5be6b-125">Jeśli korzystasz z sieci VPN, a proces logowania wylogowania zakończy działanie połączenia z domeną, możesz wyzwolić rejestrację ręcznie:</span><span class="sxs-lookup"><span data-stu-id="5be6b-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="5be6b-126">Wydaj dsregcmd/Join lokalnie na monit administratora lub zdalnie za pośrednictwem PSExec na Twój komputer.</span><span class="sxs-lookup"><span data-stu-id="5be6b-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="5be6b-127">Na przykład PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="5be6b-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="5be6b-128">Aby uzyskać więcej informacji o problemach z dołączaniem hybrydowym, zobacz [Rozwiązywanie problemów z urządzeniami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="5be6b-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
