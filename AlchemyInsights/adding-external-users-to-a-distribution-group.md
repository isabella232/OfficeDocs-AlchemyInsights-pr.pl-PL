---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660802"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="8cd10-102">Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej</span><span class="sxs-lookup"><span data-stu-id="8cd10-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="8cd10-103">Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:</span><span class="sxs-lookup"><span data-stu-id="8cd10-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="8cd10-104">Tworzenie kontaktu poczty dla użytkownika zewnętrznego:</span><span class="sxs-lookup"><span data-stu-id="8cd10-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="8cd10-105">W Centrum administracyjnym przejdź do **użytkowników** > strony[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="8cd10-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="8cd10-106">Wybierz opcję **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="8cd10-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="8cd10-107">Wpisz informacje dotyczące kontaktu i wybierz polecenie **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="8cd10-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="8cd10-108">Dodaj kontakt poczty do Twojego DG:</span><span class="sxs-lookup"><span data-stu-id="8cd10-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="8cd10-109">W Centrum administracyjnego, przejdź do **grupy** > strony[grupy](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="8cd10-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="8cd10-110">Znajdź DG, którego chcesz dodać użytkownika zewnętrznego do i zaznacz ją, aby otworzyć okno dialogowe Edytuj.</span><span class="sxs-lookup"><span data-stu-id="8cd10-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="8cd10-111">Na karcie **Członkowie** wybierz **Wyświetl wszystkie i Zarządzaj członkami**.</span><span class="sxs-lookup"><span data-stu-id="8cd10-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="8cd10-112">Wybierz **Dodaj członków**.</span><span class="sxs-lookup"><span data-stu-id="8cd10-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="8cd10-113">Wybierz kontakt poczty został utworzony w poprzednim kroku, a następnie wybierz przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="8cd10-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="8cd10-114">Jeśli po wykonaniu tych czynności użytkownika zewnętrznego, nie można wysłać wiadomości e-mail do dyrekcji generalnej lub nie otrzymywać wiadomości e-mail z niego, możliwe, że DG jest oznaczona zezwalają tylko wiadomości e-mail od użytkowników wewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="8cd10-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="8cd10-115">Można sprawdzić tę konfigurację i naprawić go zgodnie ze wskazówkami wyświetlanymi [w tym miejscu](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="8cd10-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="8cd10-116">**Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy jest "Grupa Office 365" zamiast "Grupa dystrybucyjna."</span><span class="sxs-lookup"><span data-stu-id="8cd10-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="8cd10-117">Jeśli tak się stanie, można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="8cd10-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="8cd10-118">W [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)znajdują się szczegółowe informacje dotyczące usługi Office 365 grupy gości, jak również instrukcje dotyczące dodawania zewnętrznego gośćmi.</span><span class="sxs-lookup"><span data-stu-id="8cd10-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  