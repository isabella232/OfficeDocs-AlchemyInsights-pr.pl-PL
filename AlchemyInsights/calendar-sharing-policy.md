---
title: 618 zasady udostępniania kalendarza
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684240"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="bebd5-102">Błąd zasad podczas udostępniania kalendarza</span><span class="sxs-lookup"><span data-stu-id="bebd5-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="bebd5-103">Wykonaj dowolną z następujących czynności, stosownie do sytuacji:</span><span class="sxs-lookup"><span data-stu-id="bebd5-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="bebd5-104">Nawiązywanie połączenia z usługą Exchange Online przy użyciu zdalnego programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bebd5-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="bebd5-105">Aby uzyskać więcej informacji, zobacz [łączenie się z usługą Exchange Online przy użyciu zdalnego programu PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="bebd5-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="bebd5-106">Na serwerze lokalnym Otwórz powłokę zarządzania programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="bebd5-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="bebd5-107">Określ zasady udostępniania przypisane do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="bebd5-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="bebd5-108">Aby to zrobić, uruchom następujące polecenie i zanotuj zwrócone zasady:</span><span class="sxs-lookup"><span data-stu-id="bebd5-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="bebd5-109">Zaktualizuj zasady udostępniania dla użytkownika.</span><span class="sxs-lookup"><span data-stu-id="bebd5-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="bebd5-110">Aby to zrobić, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="bebd5-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="bebd5-111">Otwórz Centrum administracyjne programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="bebd5-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="bebd5-112">Kliknij pozycję **organizacja**, a następnie kliknij dwukrotnie zasadę przypisaną do użytkownika w obszarze **udostępnianie indywidualne**.</span><span class="sxs-lookup"><span data-stu-id="bebd5-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="bebd5-113">Są to zasady zwrócone w kroku 2.</span><span class="sxs-lookup"><span data-stu-id="bebd5-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="bebd5-114">Na stronie reguła udostępniania wybierz poziom udostępniania kalendarza, dla którego chcesz zezwolić na **Określanie informacji, które chcesz udostępnić**. Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="bebd5-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="bebd5-115">Aby uzyskać więcej informacji, zobacz: ["zasady nie zezwalają na udzielanie uprawnień na tym poziomie do jednego lub większej liczby adresatów", gdy użytkownik próbuje udostępnić kalendarz](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="bebd5-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
