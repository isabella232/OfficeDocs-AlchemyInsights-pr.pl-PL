---
title: Urządzenie w stanie oczekiwania
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679987"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="358b4-102">Urządzenie w stanie oczekiwania</span><span class="sxs-lookup"><span data-stu-id="358b4-102">Device in pending state</span></span>

<span data-ttu-id="358b4-103">**Dotyczących**</span><span class="sxs-lookup"><span data-stu-id="358b4-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="358b4-104">Jeśli konfigurujesz rejestracje urządzeń po raz pierwszy, upewnij się, że zostały przejrzane [wprowadzenie do zarządzania urządzeniami w usłudze Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , które pomogą Ci w tym, jak uzyskać urządzenia objęte kontrolą usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="358b4-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="358b4-105">Jeśli rejestrujesz urządzenia w usłudze Azure AD bezpośrednio i rejestrujesz je w usłudze Intune, musisz upewnić się, że [skonfigurowano usługę Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , a w pierwszej kolejności należy wprowadzić [licencję](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="358b4-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="358b4-106">Upewnij się, że masz autoryzację do wykonywania operacji w usłudze Azure AD i w lokalnej usłudze AD.</span><span class="sxs-lookup"><span data-stu-id="358b4-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="358b4-107">Tylko administrator globalny w usłudze Azure AD może zarządzać ustawieniami rejestracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="358b4-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="358b4-108">Ponadto w przypadku konfigurowania rejestracji automatycznej w lokalnej usłudze Active Directory musisz być administratorem usługi Active Directory i usługami AD FS (jeśli jest dostępna).</span><span class="sxs-lookup"><span data-stu-id="358b4-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="358b4-109">Proces rejestracji hybrydowej dołączania Azure AD wymaga, aby urządzenia były w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="358b4-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="358b4-110">Działa również w sieci VPN, ale istnieją pewne zastrzeżenia.</span><span class="sxs-lookup"><span data-stu-id="358b4-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="358b4-111">Mamy do tego, aby klienci musieli uzyskać pomoc w rozwiązywaniu problemów dotyczących procesu rejestracji hybrydowej funkcji dołączania usługi Azure AD w ramach zdalnego środowiska roboczego.</span><span class="sxs-lookup"><span data-stu-id="358b4-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="358b4-112">**Środowisko uwierzytelniania w chmurze (Korzystanie z synchronizacji skrótu hasła w usłudze Azure AD lub uwierzytelniania przekazujące)**</span><span class="sxs-lookup"><span data-stu-id="358b4-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="358b4-113">Ten przepływ rejestracji jest również nazywany "przyłączeniem do synchronizacji".</span><span class="sxs-lookup"><span data-stu-id="358b4-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="358b4-114">Poniżej przedstawiono podział na to, co się dzieje w trakcie procesu rejestracji:</span><span class="sxs-lookup"><span data-stu-id="358b4-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="358b4-115">System Windows 10 odnajduje rekord punktu połączenia usługi (SCP), gdy użytkownik loguje się do urządzenia.</span><span class="sxs-lookup"><span data-stu-id="358b4-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="358b4-116">Urządzenie najpierw usiłuje pobrać informacje o dzierżawie ze strony klienta usługi SCP w rejestrze [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="358b4-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="358b4-117">Aby uzyskać więcej informacji, zobacz [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="358b4-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="358b4-118">Jeśli to nie uda, urządzenie komunikuje się z lokalną usługą Active Directory, aby uzyskać informacje o dzierżawie z punktu połączenia usługi.</span><span class="sxs-lookup"><span data-stu-id="358b4-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="358b4-119">Aby zweryfikować punkt SCP, należy odwołać się do tego [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="358b4-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="358b4-120">Zalecamy włączenie punktu połączenia usługi w usłudze Active Directory i korzystanie tylko z usługi SCP po stronie klienta w celu wstępnego sprawdzania poprawności.</span><span class="sxs-lookup"><span data-stu-id="358b4-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="358b4-121">System Windows 10 próbuje komunikować się z usługą Azure AD w kontekście systemowym, aby uwierzytelnić się w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="358b4-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="358b4-122">Możesz sprawdzić, czy urządzenie może uzyskać dostęp do zasobów firmy Microsoft w ramach konta system przy użyciu [skryptu łączności urządzenia testowego](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="358b4-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="358b4-123">System Windows 10 generuje certyfikat z podpisem własnym i przechowuje go w obszarze obiektu komputer w usłudze Active Directory lokalnego.</span><span class="sxs-lookup"><span data-stu-id="358b4-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="358b4-124">Wymaga to, aby kontroler domeny był oparty na linii.</span><span class="sxs-lookup"><span data-stu-id="358b4-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="358b4-125">Obiekt urządzenia z certyfikatem zostanie zsynchronizowany z usługą Azure AD za pośrednictwem usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="358b4-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="358b4-126">Cykl synchronizacji jest domyślnie co 30 minut, ale zależy od konfiguracji usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="358b4-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="358b4-127">Aby uzyskać więcej informacji, zapoznaj się z tym [dokumentem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="358b4-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="358b4-128">Na tym etapie powinno być możliwe wyświetlenie urządzenia subject w stanie "**oczekujące**" w obszarze Kaseta urządzenia usługi Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="358b4-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="358b4-129">Po następnym zalogowaniu się użytkownika do systemu Windows 10 rejestracja zostanie zakończona.</span><span class="sxs-lookup"><span data-stu-id="358b4-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="358b4-130">Jeśli korzystasz z sieci VPN, a wylogowanie/logowanie zakończy łączność z domeną, możesz wyzwolić rejestrację ręcznie.</span><span class="sxs-lookup"><span data-stu-id="358b4-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="358b4-131">W tym celu:</span><span class="sxs-lookup"><span data-stu-id="358b4-131">To do that:</span></span>
    >
    > <span data-ttu-id="358b4-132">Wygeneruj `dsregcmd /join` lokalnie monit administratora lub zdalnie, korzystając z PSExec na komputerze.</span><span class="sxs-lookup"><span data-stu-id="358b4-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="358b4-133">Na przykład: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="358b4-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="358b4-134">Aby poznać typowe problemy dotyczące rejestracji urządzeń usługi Azure Active Directory, zobacz [często zadawane pytania dotyczące urządzeń](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="358b4-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
