---
title: 618 Zasady udostępniania kalendarza
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373009"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="8b712-102">Błąd zasad podczas udostępniania kalendarza</span><span class="sxs-lookup"><span data-stu-id="8b712-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="8b712-103">Wykonaj jedną z następujących czynności, odpowiednio do sytuacji:</span><span class="sxs-lookup"><span data-stu-id="8b712-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="8b712-104">Połącz się z usługą Exchange Online przy użyciu programu Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8b712-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="8b712-105">Aby uzyskać więcej informacji, zobacz [Łączenie się z usługą Exchange Online przy użyciu programu Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8b712-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="8b712-106">Na serwerze lokalnym otwórz powłokę zarządzania programem Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b712-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="8b712-107">Określ zasady udostępniania przypisane do użytkownika.</span><span class="sxs-lookup"><span data-stu-id="8b712-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="8b712-108">Aby to zrobić, uruchom następujące polecenie i zanotuj zwrócone zasady:</span><span class="sxs-lookup"><span data-stu-id="8b712-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="8b712-109">Zaktualizuj zasady udostępniania dla użytkownika.</span><span class="sxs-lookup"><span data-stu-id="8b712-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="8b712-110">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8b712-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="8b712-111">Otwórz centrum administracyjne programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b712-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="8b712-112">Kliknij pozycję **Organizacja**, a następnie kliknij dwukrotnie zasadę przypisaną do użytkownika w obszarze **Udostępnianie indywidualne**.</span><span class="sxs-lookup"><span data-stu-id="8b712-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="8b712-113">Jest to zasada, która została zwrócona w kroku 2.</span><span class="sxs-lookup"><span data-stu-id="8b712-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="8b712-114">Na stronie Reguła udostępniania wybierz poziom udostępniania kalendarza, na który chcesz zezwolić w obszarze **Określanie informacji, które chcesz udostępnić;** kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="8b712-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="8b712-115">Aby uzyskać więcej informacji, zobacz: ["Zasady nie zezwalają na udzielanie uprawnień na tym poziomie jednemu lub większej liczbie adresatów" błędu podczas próby udostępnienia kalendarza](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)przez użytkownika .</span><span class="sxs-lookup"><span data-stu-id="8b712-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
