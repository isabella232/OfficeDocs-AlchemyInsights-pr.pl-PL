---
title: Dostęp warunkowy z urządzeniem przyłączony do domeny jest blokowany
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038109"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="de029-102">Dostęp warunkowy z urządzeniem przyłączony do domeny jest blokowany</span><span class="sxs-lookup"><span data-stu-id="de029-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="de029-103">**Wysoce zalecane narzędzia**</span><span class="sxs-lookup"><span data-stu-id="de029-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="de029-104">[Narzędzie do rozwiązywania problemów z rejestracją](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) urządzenia — narzędzie, które pomaga w rozwiązywaniu najczęstszych problemów z rejestracją urządzenia.</span><span class="sxs-lookup"><span data-stu-id="de029-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="de029-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — skrypt, który pomaga zapewnić, że urządzenie może uzyskać dostęp do punktów końcowych rejestracji urządzeń w ramach konta systemowego.</span><span class="sxs-lookup"><span data-stu-id="de029-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="de029-106">[Skrypt oczyszczania urządzenia usługi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) — skrypt, który umożliwia szukanie przestarzałych urządzeń i zarządzanie nimi w środowisku.</span><span class="sxs-lookup"><span data-stu-id="de029-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="de029-107">Oto kilka typowych powodów, dla których dostęp warunkowy może powodować niepowodzenie działania urządzenia, które przyłączyło się do domeny (hybrydowa usługa Azure AD).</span><span class="sxs-lookup"><span data-stu-id="de029-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="de029-108">**Na urządzeniu nie ma narzędzia Azure AD PRT** — musisz się upewnić, że urządzenie ma token odświeżania podstawowego usługi Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="de029-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="de029-109">Aby uzyskać więcej informacji na temat prt, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="de029-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="de029-110">Aby sprawdzić, czy masz narzędzie Azure AD PRT, uruchom polecenie na urządzeniu i sprawdź, czy `dsregcmd/status` "AzureAdPrt" ma pozycję "YES".</span><span class="sxs-lookup"><span data-stu-id="de029-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="de029-111">Jeśli argument "AzureAdPrt" ma stan "NIE", sprawdź następujące kwestie:</span><span class="sxs-lookup"><span data-stu-id="de029-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="de029-112">Niezależnie od tego, czy masz środowisko **federacyjnych** z usługami AD FS i jest to nieosiągalne w sieciach domowych użytkowników: W takim przypadku upewnij się, że punkty końcowe "nazwa_użytkownikamixed" są dostępne z ekstranetu.</span><span class="sxs-lookup"><span data-stu-id="de029-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="de029-113">Jeśli usługi AD FS są za siecią VPN, upewnij się, że użytkownicy łączą się z siecią VPN i zalogują się ponownie na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="de029-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="de029-114">Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="de029-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="de029-115">**Czy usługa TPM** urządzenia jest błędna, a zatem nie może uwierzytelnić urządzenia: sprawdź, czy moduł TPM ma stan "Gotowe".</span><span class="sxs-lookup"><span data-stu-id="de029-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="de029-116">Jeśli nie, uruchom program i poczekaj, aby urządzenie ponownie `dsregcmd/leave` dołączyło do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de029-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="de029-117">Następnie spróbuj ponownie.</span><span class="sxs-lookup"><span data-stu-id="de029-117">Then, try again.</span></span> <span data-ttu-id="de029-118">Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="de029-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="de029-119">**Korzystasz z zewnętrznego** dostawcy tożsamości, który nie obsługuje WS-Trust protokołu .</span><span class="sxs-lookup"><span data-stu-id="de029-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="de029-120">Jak opisano w naszych pracach, w tym przypadku hybrydowe urządzenia przyłączone do usługi Azure AD nie mogą działać.</span><span class="sxs-lookup"><span data-stu-id="de029-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="de029-121">Skontaktuj się z dostawcą tożsamości, aby uzyskać pomoc techniczną.</span><span class="sxs-lookup"><span data-stu-id="de029-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="de029-122">Użytkownicy korzystają z przeglądarki Chrome bez kont systemu **Windows 10** lub rozszerzenia pakietu Office Chrome nie używają automatycznie prt na urządzeniach przyłączony do AAD lub przyłączony hybrydowych **—AAD:** Spowoduje to niepowodzenie wszystkich zasad dostępu warunkowego opartych na urządzeniu z wyświetlonym komunikatem o błędzie "Niezarejestrowane urządzenie".</span><span class="sxs-lookup"><span data-stu-id="de029-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="de029-123">Aby prawidłowo używać przeglądarki Chrome, musisz zainstalować "Konta systemu Windows 10" lub "Rozszerzenie pakietu Office dla przeglądarki Chrome użytkowników" za pomocą programu SCCM lub Intune.</span><span class="sxs-lookup"><span data-stu-id="de029-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="de029-124">Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="de029-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="de029-125">Jeśli nie jest możliwe zdalne wypychanie rozszerzenia, powiadom użytkowników, aby ręcznie zainstalują jedno z powyższych rozszerzeń, aby uzyskać dostęp do aplikacji korzystających z dostępu warunkowego opartego na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="de029-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="de029-126">Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="de029-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="de029-127">Urządzenie zostało poprawnie sprzężenia hybrydowego usługi **Azure AD, ale** zostało przypadkowo usunięte lub wyłączone ze względu na zmiany synchronizacji w programie Azure AD Connect lub w portalu Azure: W takim przypadku obiekt urządzenia nie jest już rozpoznawany jako urządzenie w pełni sprzężenia, nawet jeśli stan "AzureAdJoined" i "PRT" są wyświetlane jako prawidłowe na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="de029-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="de029-128">Aby rozwiązać ten problem, uruchom na urządzeniach, których to dotyczy, i pozwól im ponownie dołączyć `dsregcmd/leave` do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de029-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="de029-129">Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="de029-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="de029-130">Jeśli twoje urządzenia znajdują się w aktualizacji systemu Windows 10, 1809, z serwerem proxy w sieci VPN/chmurze i widzą problemy z stanem "AzureAdPrt" lub dowolną aplikacją z problemem z logowaniem jednokrotnym (program Outlook nie łączy się ze skrzynką pocztową, mimo że był prT), upewnij się, że masz tę poprawkę [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) lub aktualizację skumulowaną z kwietnia [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) aby zapobiec błędom PRT na tych komputerach.</span><span class="sxs-lookup"><span data-stu-id="de029-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















