---
title: Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555303"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="e1d3b-102">Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta</span><span class="sxs-lookup"><span data-stu-id="e1d3b-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="e1d3b-103">Profile certyfikatów klienta usługi Intune NDES/SCEP i PKCS/PFX są powszechnie używane w połączeniu z innymi typami profili, takimi jak Wifi, VPN i poczta e-mail, aby umożliwić użytkownikom uwierzytelnienie się w zasobach firmowych.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="e1d3b-104">Gdy te typy profili są połączone z profilem certyfikatu klienta są zależne od pomyślnego wdrożenia tego profilu.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="e1d3b-105">Początkowa konfiguracja infrastruktury i skojarzona konfiguracja profilu certyfikatu klienta często wymagają rozwiązywania problemów.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="e1d3b-106">Aby uzyskać przewodnik krok po kroku dotyczący pomyślnej konfiguracji łącznika NDES i wskazówek dotyczących rozwiązywania problemów w celu wyizolowania problemów z wdrażaniem certyfikatów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="e1d3b-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="e1d3b-107">Konfigurowanie infrastruktury do obsługi narzędzia SCEP w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="e1d3b-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="e1d3b-108">Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e1d3b-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="e1d3b-109">Użyj skryptów programu PowerShell, do których odwołuje się skrypty programu PowerShell, aby zweryfikować konfigurację.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="e1d3b-110">Aby uzyskać więcej informacji, zobacz [Skrypty weryfikacji łącznika łącznika usługi Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="e1d3b-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="e1d3b-111">**Inne typowe problemy**</span><span class="sxs-lookup"><span data-stu-id="e1d3b-111">**Other common issues**</span></span>

<span data-ttu-id="e1d3b-112">**Podczas próby zainstalowania łącznika certyfikatu usługi Intune na serwerze łącznika NDES otrzymuję komunikat "Nie można zweryfikować hasła w żądaniu certyfikatu. Być może był już używany. Uzyskaj nowe hasło do przesłania z tym żądaniem."**</span><span class="sxs-lookup"><span data-stu-id="e1d3b-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="e1d3b-113">Ten komunikat oznacza, że należy uruchomić instalację łącznika certyfikatu jako administrator.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="e1d3b-114">W niektórych środowiskach serwery uruchamiane jako certyfikat usługi Intune muszą używać serwera proxy do łączenia się z usługą Intune, dlatego łącznik certyfikatów musi używać serwera proxy.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="e1d3b-115">W pewnych okolicznościach łącznik NDES ignoruje skonfigurowane ustawienia serwera proxy i może być konieczne skonfigurowanie ustawień serwera proxy podczas uruchamiania w kontekście zabezpieczeń systemu localsystem.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="e1d3b-116">Rozwiązaniem jest uruchomienie programu Internet Explorer jako system i skonfigurowanie serwera proxy w programie IE.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="e1d3b-117">Po ponownym uruchomieniu usługi łącznika usługi Intune łącznik ndes łącznik łączy się z usługą Intune.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="e1d3b-118">**Urządzenia użytkownika nie otrzymują już certyfikatów SCEP od NDES.**</span><span class="sxs-lookup"><span data-stu-id="e1d3b-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="e1d3b-119">Możliwe, że certyfikat uwierzytelniania klienta wystawiony serwerowi NDES i określony podczas instalacji łącznika NDES wygasł lub jej brakuje.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="e1d3b-120">Aby rozwiązać:</span><span class="sxs-lookup"><span data-stu-id="e1d3b-120">To resolve:</span></span> 
 
1. <span data-ttu-id="e1d3b-121">Odinstaluj łącznik NDES.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="e1d3b-122">Te szczegóły można użyć, aby zażądać nowego certyfikatu uwierzytelniania klienta lub certyfikatu uwierzytelniania serwera:</span><span class="sxs-lookup"><span data-stu-id="e1d3b-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="e1d3b-123">Nazwa podmiotu: CN =external fqdn</span><span class="sxs-lookup"><span data-stu-id="e1d3b-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="e1d3b-124">Alternatywna nazwa podmiotu (obie są wymagane): DNS=external fqdn, DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="e1d3b-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="e1d3b-125">Zainstaluj ponownie łącznik NDES z nowym certyfikatem.</span><span class="sxs-lookup"><span data-stu-id="e1d3b-125">Reinstall the NDES connector with the new certificate.</span></span>