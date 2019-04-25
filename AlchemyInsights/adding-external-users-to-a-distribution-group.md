---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej?
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398468"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="10cce-102">Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej?</span><span class="sxs-lookup"><span data-stu-id="10cce-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="10cce-103">Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem krok 2:</span><span class="sxs-lookup"><span data-stu-id="10cce-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="10cce-104">Tworzenie kontaktu poczty dla użytkownika zewnętrznego:</span><span class="sxs-lookup"><span data-stu-id="10cce-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="10cce-105">Kliknij [tutaj](https://admin.microsoft.com/adminportal/home#/Contact) aby przejść do strony edycji kontaktu w portalu administratora.</span><span class="sxs-lookup"><span data-stu-id="10cce-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="10cce-106">Wybierz polecenie **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="10cce-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="10cce-107">Wpisz informacje dotyczące kontaktu, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="10cce-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="10cce-108">Dodaj kontakt poczty do Twojego DG:</span><span class="sxs-lookup"><span data-stu-id="10cce-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="10cce-109">Kliknij [tutaj](https://admin.microsoft.com/adminportal/home#/groups) , aby przejść do strony grupy.</span><span class="sxs-lookup"><span data-stu-id="10cce-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="10cce-110">Znajdź DG chcesz dodać użytkownika zewnętrznego i kliknij go, aby otworzyć okno dialogowe Edytuj.</span><span class="sxs-lookup"><span data-stu-id="10cce-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="10cce-111">Kliknij przycisk **Edytuj** na liście **członków** .</span><span class="sxs-lookup"><span data-stu-id="10cce-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="10cce-112">Wybierz polecenie **Dodaj członków**.</span><span class="sxs-lookup"><span data-stu-id="10cce-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="10cce-113">Wybierz kontakt poczty został utworzony w poprzednim kroku, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="10cce-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="10cce-114">Jeśli nawet po wykonaniu tych czynności użytkownika zewnętrznego, nie można wysłać wiadomości e-mail do dyrekcji generalnej lub nie otrzymywać wiadomości e-mail z niego, można go, że DG jest oznaczona zezwalają tylko wiadomości e-mail od użytkowników wewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="10cce-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="10cce-115">Można sprawdzić tę konfigurację i naprawić go zgodnie ze wskazówkami wyświetlanymi [w tym miejscu](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span><span class="sxs-lookup"><span data-stu-id="10cce-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="10cce-116">**Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy jest "Grupa Office 365" zamiast "Grupa dystrybucyjna."</span><span class="sxs-lookup"><span data-stu-id="10cce-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="10cce-117">Jeśli tak się stanie, można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook lub programu Outlook w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="10cce-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="10cce-118">W [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)znajdują się szczegółowe wyjaśnienie na O365 grupy gości, jak również instrukcje dotyczące dodawania zewnętrznego gośćmi.</span><span class="sxs-lookup"><span data-stu-id="10cce-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

