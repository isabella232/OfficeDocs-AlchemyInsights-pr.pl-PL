---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663523"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d384f-102">Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej</span><span class="sxs-lookup"><span data-stu-id="d384f-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d384f-103">Dodanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:</span><span class="sxs-lookup"><span data-stu-id="d384f-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d384f-104">Tworzenie kontaktu poczty dla użytkownika zewnętrznego:</span><span class="sxs-lookup"><span data-stu-id="d384f-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d384f-105">W centrum administracyjnym przejdź do strony Kontakty **użytkowników**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="d384f-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d384f-106">Wybierz pozycję **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="d384f-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d384f-107">Wpisz informacje dotyczące kontaktu i wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="d384f-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d384f-108">Dodaj kontakt z pocztą do swojej DG:</span><span class="sxs-lookup"><span data-stu-id="d384f-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d384f-109">W centrum administracyjnym przejdź do strony grupy **grup**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="d384f-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d384f-110">Znajdź DG, do którego chcesz dodać użytkownika zewnętrznego, a następnie wybierz go, aby otworzyć okno dialogowe Edytowanie.</span><span class="sxs-lookup"><span data-stu-id="d384f-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d384f-111">Na karcie **Członkowie** wybierz pozycję **Pokaż wszystkich członków i zarządzaj nimi**.</span><span class="sxs-lookup"><span data-stu-id="d384f-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d384f-112">Wybierz pozycję **Dodaj członków**.</span><span class="sxs-lookup"><span data-stu-id="d384f-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d384f-113">Wybierz kontakt poczty utworzony w poprzednim kroku, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="d384f-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d384f-114">Jeśli po wykonaniu tych czynności użytkownicy zewnętrzni nie będą mogli wysyłać wiadomości e-mail do tej DG ani odbierać wiadomości e-mail z tej usługi, może to oznaczać, że ta DG jest oznaczona jako przeznaczona tylko do obsługi wiadomości e-mail od użytkowników wewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="d384f-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d384f-115">Możesz sprawdzić tę konfigurację i rozwiązać ją, postępując zgodnie z [instrukcjami.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="d384f-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="d384f-116">**Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ Twojej grupy to "Microsoft 365 Group" zamiast "Grupa dystrybucyjna".</span><span class="sxs-lookup"><span data-stu-id="d384f-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d384f-117">W takim przypadku użytkownik zewnętrzny może dodać użytkownika zewnętrznego bezpośrednio do grupy z poziomu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="d384f-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d384f-118">Szczegółowe informacje na temat Gości grupowych Microsoft 365 oraz instrukcje dotyczące dodawania zewnętrznych Gości można znaleźć w [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="d384f-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  