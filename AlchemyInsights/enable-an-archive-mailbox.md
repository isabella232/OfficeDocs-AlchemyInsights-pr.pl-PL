---
title: Włączanie archiwum Skrzynka pocztowa
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811715"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="4cdaf-102">Włączanie archiwum Skrzynka pocztowa</span><span class="sxs-lookup"><span data-stu-id="4cdaf-102">Enable an archive mailbox</span></span>

<span data-ttu-id="4cdaf-103">Jeśli chcesz, aby na bieżąco uruchamiać zautomatyzowane testy w celu zapewnienia, że można skonfigurować archiwalną skrzynkę pocztową, wybierz przycisk Wstecz <--u góry tej strony, a następnie wprowadź adres e-mail tego konta.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="4cdaf-104">Archiwizowanie skrzynek pocztowych w programie Microsoft 365 (nazywanych też *archiwami online* lub *archiwami miejscowymi*) zapewnia użytkownikom dodatkowe miejsce do magazynowania wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="4cdaf-105">Użytkownicy mogą przenosić lub kopiować elementy do ich archiwalnej skrzynki pocztowej, a administratorzy mogą tworzyć Zasady archiwizacji, które automatycznie przenoszą elementy do archiwum skrzynek pocztowych.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="4cdaf-106">Poniżej opisano, jak utworzyć archiwalną skrzynkę pocztową:</span><span class="sxs-lookup"><span data-stu-id="4cdaf-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="4cdaf-107">Przejdź do witryny [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="4cdaf-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="4cdaf-108">Zaloguj się do aplikacji Microsoft 365 przy użyciu konta administratora.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="4cdaf-109">W lewym okienku &amp; Centrum zgodności zabezpieczeń wybierz pozycję Archiwum **zarządzania informacjami** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="4cdaf-110">Wybierz użytkownika, którego Skrzynka pocztowa ma zostać włączona.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="4cdaf-111">W okienku szczegółów po prawej stronie kliknij pozycję **Włącz** , a następnie kliknij przycisk **tak** w komunikacie ostrzegawczym, aby włączyć archiwum Skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="4cdaf-112">Można też włączyć zbiorczo obsługę skrzynek pocztowych, wybierając wielu użytkowników (przy użyciu klawiszy **SHIFT** lub **Ctrl** ), a następnie klikając pozycję **Włącz** w okienku szczegółów.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="4cdaf-113">Udostępnione skrzynki pocztowe</span><span class="sxs-lookup"><span data-stu-id="4cdaf-113">Shared mailboxes</span></span>

<span data-ttu-id="4cdaf-114">Aby włączyć archiwum do udostępnionej skrzynki pocztowej, wymagana jest licencja na usługę Exchange Online (plan 2) lub licencję Exchange Online (plan 1) z licencją usługi Exchange Online do archiwizacji.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="4cdaf-115">Aby włączyć archiwum do udostępnionej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="4cdaf-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="4cdaf-116">Przejdź do [Centrum administracyjnego programu Exchange](https://outlook.office365.com/ecp) i zaloguj się przy użyciu konta administratora.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="4cdaf-117">Przejdź do **adresatów**  >  **udostępnionych**.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="4cdaf-118">Wybierz udostępnioną skrzynkę pocztową.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="4cdaf-119">W okienku szczegółów po prawej stronie w obszarze **archiwum miejscowe**kliknij pozycję **Włącz**, a następnie kliknij pozycję **tak** , aby włączyć archiwum Skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="4cdaf-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="4cdaf-120">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="4cdaf-120">For more information, see:</span></span>
  
- [<span data-ttu-id="4cdaf-121">Włączanie archiwum skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="4cdaf-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="4cdaf-122">Konfigurowanie zasad archiwizacji i usuwania</span><span class="sxs-lookup"><span data-stu-id="4cdaf-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
