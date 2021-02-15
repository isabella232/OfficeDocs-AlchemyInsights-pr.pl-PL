---
title: Pisanie zwrotne hasła nie działa
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243518"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="8979d-102">Pisanie zwrotne hasła nie działa</span><span class="sxs-lookup"><span data-stu-id="8979d-102">Password Writeback is not working</span></span>

<span data-ttu-id="8979d-103">**Mam problemy z konfiguracją zapisu hasła**</span><span class="sxs-lookup"><span data-stu-id="8979d-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="8979d-104">Funkcja zwrotu hasła jest funkcją klasy premium.</span><span class="sxs-lookup"><span data-stu-id="8979d-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="8979d-105">Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:</span><span class="sxs-lookup"><span data-stu-id="8979d-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="8979d-106">W organizacji musi być przypisana co najmniej jedna licencja</span><span class="sxs-lookup"><span data-stu-id="8979d-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="8979d-107">**Tylko użytkownicy w chmurze** — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="8979d-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="8979d-108">**Użytkownicy chmury i/lub** lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="8979d-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="8979d-109">Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="8979d-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="8979d-110">Masz co najmniej jedno konto administratora i jedno testowe konto użytkownika z jedną odpowiednią licencją.</span><span class="sxs-lookup"><span data-stu-id="8979d-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="8979d-111">Aby działało, należy połączyć program Azure AD Connect Kontroler domeny podstawowym emulatorem hasła.</span><span class="sxs-lookup"><span data-stu-id="8979d-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="8979d-112">Program Azure AD Connect można skonfigurować do używania klucza  podstawowego Kontroler domeny klikając prawym przyciskiem myszy właściwości łącznika synchronizacji usługi Active Directory, a następnie wybierając pozycję Skonfiguruj **partycje katalogowe.**</span><span class="sxs-lookup"><span data-stu-id="8979d-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="8979d-113">W tym miejscu poszukaj sekcji **ustawień** połączenia kontrolera domeny i zaznacz pole wyboru "Użyj **tylko preferowanych kontrolerów domen".**</span><span class="sxs-lookup"><span data-stu-id="8979d-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="8979d-114">Jeśli preferowany kontroler domeny nie jest emulatorem pdc, program Azure AD Connect nadal będzie się kontaktował z tym kontrolerem w celu zapisu hasła.</span><span class="sxs-lookup"><span data-stu-id="8979d-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="8979d-115">Resetowanie hasła zostało skonfigurowane i włączone w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="8979d-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="8979d-116">Aby uzyskać więcej informacji, zobacz "Umożliwianie użytkownikom resetowania haseł usługi [Azure AD".](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="8979d-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="8979d-117">Upewnij się, że konto administratora używane do włączania funkcji zapisu zwrotnego haseł jest kontem administratora chmury (utworzone w usłudze Azure AD, a nie w lokalnej usłudze AD)</span><span class="sxs-lookup"><span data-stu-id="8979d-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="8979d-118">Masz jedno lub wielo lassowe wdrożenie lokalne usługi AD z zainstalowanymi najnowszymi pakietami Service Pack dla systemów Windows Server 2008 R2, Windows Server 2012 lub Windows Server 2012 R2</span><span class="sxs-lookup"><span data-stu-id="8979d-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="8979d-119">Masz zainstalowane narzędzie Azure AD Connect i masz przygotowane środowisko usługi AD do synchronizacji z chmurą.</span><span class="sxs-lookup"><span data-stu-id="8979d-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="8979d-120">Przed przetestowaniem zapisu hasła upewnij się, że najpierw ukończono pełne importowanie i pełną synchronizację z usług AD i Azure AD w programie Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8979d-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="8979d-121">Aby dowiedzieć się więcej, zobacz, jak wykonać pełną synchronizację i [pełne importowanie w programie Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="8979d-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="8979d-122">**Mam problem z łącznością zapisu zwrotnego haseł**</span><span class="sxs-lookup"><span data-stu-id="8979d-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="8979d-123">Pobieranie i włączanie najnowszej wersji programu [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="8979d-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="8979d-124">Konfiguracja zapory: Narzędzie Azure AD Connect (1.1.443 i więcej) będzie potrzebowało wychodzącego **dostępu HTTPS** do:</span><span class="sxs-lookup"><span data-stu-id="8979d-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="8979d-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8979d-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="8979d-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="8979d-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="8979d-127">Zezwalaj na utrzymywanie bezczynnych połączeń przez co najmniej 2–3 minuty</span><span class="sxs-lookup"><span data-stu-id="8979d-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="8979d-128">**Nadal mam problemy z zapisem hasła**</span><span class="sxs-lookup"><span data-stu-id="8979d-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="8979d-129">Jeśli nadal masz problemy, spróbuj wyłączyć i ponownie włączyć usługę odzyskiwania hasła w narzędziu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8979d-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="8979d-130">Aby dowiedzieć się więcej, zobacz, jak [wyłączyć i ponownie włączyć funkcję zapisu hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="8979d-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
