---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910942"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="dd5cb-102">Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej</span><span class="sxs-lookup"><span data-stu-id="dd5cb-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="dd5cb-103">Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:</span><span class="sxs-lookup"><span data-stu-id="dd5cb-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="dd5cb-104">Utwórz kontakt poczty dla użytkownika zewnętrznego:</span><span class="sxs-lookup"><span data-stu-id="dd5cb-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="dd5cb-105">W centrum administracyjnym przejdź do strony[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) **użytkowników.** > </span><span class="sxs-lookup"><span data-stu-id="dd5cb-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="dd5cb-106">Wybierz **pozycję Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="dd5cb-107">Wpisz informacje dotyczące kontaktu i wybierz pozycję **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="dd5cb-108">Dodaj kontakt pocztowy do dyrekcji dg:</span><span class="sxs-lookup"><span data-stu-id="dd5cb-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="dd5cb-109">W centrum administracyjnym przejdź **Groups** > do strony[Grupy](https://admin.microsoft.com/adminportal/home#/groups) grup.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="dd5cb-110">Znajdź dyrekcję dg, do której chcesz dodać użytkownika zewnętrznego, i wybierz ją, aby otworzyć okno dialogowe edycji.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="dd5cb-111">Na karcie **Członkowie** wybierz pozycję **Wyświetl wszystkich członków i zarządzaj nimi.**</span><span class="sxs-lookup"><span data-stu-id="dd5cb-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="dd5cb-112">Wybierz **pozycję Dodaj członków**.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="dd5cb-113">Wybierz kontakt poczty utworzony w poprzednim kroku, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="dd5cb-114">Jeśli po wykonać te kroki użytkownicy zewnętrzni nie mogą wysyłać wiadomości e-mail do Dyrekcji DG lub nie otrzymują od niej wiadomości e-mail, może to oznaczać, że Dyrekcja DG jest oznaczona jako zezwalana tylko na wiadomości e-mail od użytkowników wewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="dd5cb-115">Możesz sprawdzić tę konfigurację i naprawić ją, postępują zgodnie ze wskazówkami [tutaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="dd5cb-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="dd5cb-116">**Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy to "Grupa microsoft 365" zamiast "Grupa dystrybucyjna".</span><span class="sxs-lookup"><span data-stu-id="dd5cb-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="dd5cb-117">W takim przypadku można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="dd5cb-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="dd5cb-118">Szczegółowe informacje na temat gości grupy Microsoft 365 oraz instrukcje dotyczące dodawania gości zewnętrznych można znaleźć w [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="dd5cb-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  