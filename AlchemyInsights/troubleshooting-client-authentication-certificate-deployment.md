---
title: Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658996"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="e57ed-102">Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta</span><span class="sxs-lookup"><span data-stu-id="e57ed-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="e57ed-103">Profile certyfikatów klienta usługi Intune NDES/SCEP i PKCS/PFX są często używane w połączeniu z innymi typami profilów, takimi jak WiFi, VPN i poczta e-mail, aby umożliwić użytkownikom uwierzytelnianie w zasobach firmowych.</span><span class="sxs-lookup"><span data-stu-id="e57ed-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="e57ed-104">Jeśli te typy profilów są połączone z profilem certyfikatu klienta, są zależne od poprawnego wdrożenia tego profilu.</span><span class="sxs-lookup"><span data-stu-id="e57ed-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="e57ed-105">Początkowa konfiguracja infrastruktury i skojarzona konfiguracja profilu certyfikatu klienta wymagają często rozwiązywania problemów.</span><span class="sxs-lookup"><span data-stu-id="e57ed-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="e57ed-106">Aby zapoznać się z przewodnikiem krok po kroku dotyczącym poprawnego konfigurowania łącznika usługi NDES i wskazówek dotyczących rozwiązywania problemów z wdrażaniem certyfikatów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="e57ed-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="e57ed-107">Konfigurowanie infrastruktury do obsługi protokołu SCEP za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="e57ed-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="e57ed-108">Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e57ed-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="e57ed-109">Używanie skryptów programu PowerShell, do których można sprawdzić konfigurację.</span><span class="sxs-lookup"><span data-stu-id="e57ed-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="e57ed-110">Aby uzyskać więcej informacji, zobacz [skrypty weryfikacji łącznika certyfikatów usługi Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="e57ed-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="e57ed-111">**Inne typowe problemy**</span><span class="sxs-lookup"><span data-stu-id="e57ed-111">**Other common issues**</span></span>

<span data-ttu-id="e57ed-112">**Gdy próbuję zainstalować łącznik certyfikatów usługi Intune na serwerze usługi NDES Connector, jest wyświetlany komunikat "nie można zweryfikować hasła w żądaniu certyfikatu. Być może został on już wykorzystany. Uzyskaj nowe hasło do przesłania za pomocą tego żądania.**</span><span class="sxs-lookup"><span data-stu-id="e57ed-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="e57ed-113">Ta wiadomość oznacza, że musisz uruchomić instalację łącznika certyfikatu jako administrator.</span><span class="sxs-lookup"><span data-stu-id="e57ed-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="e57ed-114">W niektórych środowiskach serwery, na których jest uruchomiony certyfikat usługi Intune, muszą używać serwera proxy do nawiązywania połączenia z usługą Intune, więc łącznik certyfikatów musi używać serwera proxy.</span><span class="sxs-lookup"><span data-stu-id="e57ed-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="e57ed-115">W pewnych okolicznościach łącznik usługi NDES ignoruje skonfigurowane ustawienia serwera proxy i może być konieczne skonfigurowanie ustawień serwera proxy podczas uruchamiania w kontekście zabezpieczeń LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="e57ed-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="e57ed-116">Rozwiązanie polega na uruchomieniu programu Internet Explorer w systemie i skonfigurowaniu serwera proxy w programie IE.</span><span class="sxs-lookup"><span data-stu-id="e57ed-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="e57ed-117">Po ponownym uruchomieniu usługi łącznika usługi Intune łącznik usługi NDES łączy się z usługą Intune.</span><span class="sxs-lookup"><span data-stu-id="e57ed-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="e57ed-118">**Urządzenia użytkowników nie odbierają już certyfikatów SCEP z usługi NDES.**</span><span class="sxs-lookup"><span data-stu-id="e57ed-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="e57ed-119">Możliwe, że certyfikat uwierzytelniania klienta wystawiony dla serwera NDES i określony podczas instalacji łącznika usługi NDES stracił ważność lub go brakuje.</span><span class="sxs-lookup"><span data-stu-id="e57ed-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="e57ed-120">Aby rozpoznać:</span><span class="sxs-lookup"><span data-stu-id="e57ed-120">To resolve:</span></span> 
 
1. <span data-ttu-id="e57ed-121">Odinstaluj łącznik usługi NDES.</span><span class="sxs-lookup"><span data-stu-id="e57ed-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="e57ed-122">Te szczegóły umożliwiają zażądanie nowego uwierzytelniania klienta lub certyfikatu uwierzytelniania serwera:</span><span class="sxs-lookup"><span data-stu-id="e57ed-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="e57ed-123">Nazwa podmiotu: CN = zewnętrzna nazwa FQDN</span><span class="sxs-lookup"><span data-stu-id="e57ed-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="e57ed-124">Alternatywna nazwa podmiotu (wymagane): DNS = zewnętrzna nazwa FQDN, DNS = wewnętrzna nazwa FQDN</span><span class="sxs-lookup"><span data-stu-id="e57ed-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="e57ed-125">Ponownie zainstaluj łącznik usługi NDES z nowym certyfikatem.</span><span class="sxs-lookup"><span data-stu-id="e57ed-125">Reinstall the NDES connector with the new certificate.</span></span>