---
title: Tworzenie zasad udostępniania w celu umożliwienia użytkownikom udostępniania kalendarza osobom spoza organizacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816282"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="132f4-102">Tworzenie zasad udostępniania w celu umożliwienia użytkownikom udostępniania kalendarza osobom spoza organizacji</span><span class="sxs-lookup"><span data-stu-id="132f4-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="132f4-103">Z pulpitu nawigacyjnego centrum administracyjnego platformy Microsoft 365 przejdź do **Administrator** > **Usługa Exchange**.</span><span class="sxs-lookup"><span data-stu-id="132f4-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="132f4-104">Przejdź do pozycji **Organizacja** > **Udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="132f4-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="132f4-105">W widoku listy w obszarze **Udostępnianie indywidualne** kliknij pozycję **Nowy** .</span><span class="sxs-lookup"><span data-stu-id="132f4-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="132f4-106">W **polu Nazwa zasad** w nowych zasadach udostępniania wpisz przyjazną nazwę **zasad** udostępniania.</span><span class="sxs-lookup"><span data-stu-id="132f4-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="132f4-107">Kliknij **przycisk Dodaj,**  aby zdefiniować reguły udostępniania zasad.</span><span class="sxs-lookup"><span data-stu-id="132f4-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="132f4-108">W **regułach** udostępniania wybierz jedną z następujących opcji, aby określić domeny, którym chcesz udostępnić elementy:</span><span class="sxs-lookup"><span data-stu-id="132f4-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="132f4-109">**Udostępnianie wszystkim domenom**</span><span class="sxs-lookup"><span data-stu-id="132f4-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="132f4-110">**Udostępnianie określonej domeny**</span><span class="sxs-lookup"><span data-stu-id="132f4-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="132f4-111">Jeśli wybierzesz **pozycję Udostępnianie określonej domenie,** wpisz nazwę domeny, której chcesz udostępnić.</span><span class="sxs-lookup"><span data-stu-id="132f4-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="132f4-112">Jeśli chcesz wprowadzić więcej niż jedną domenę dla tych zasad udostępniania, zapisz ustawienia dla pierwszej domeny, a następnie edytuj reguły udostępniania, aby dodać więcej domen.</span><span class="sxs-lookup"><span data-stu-id="132f4-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="132f4-113">Aby określić informacje, które mogą być udostępniane, zaznacz pole **wyboru Udostępnij folder** kalendarza, a następnie wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="132f4-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="132f4-114">**Informacje o stanie wolny lub zajęty dla kalendarza zawierające tylko określenie czasu**</span><span class="sxs-lookup"><span data-stu-id="132f4-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="132f4-115">**Informacje wolny/zajęty z kalendarza z godziną, tematem i lokalizacją**</span><span class="sxs-lookup"><span data-stu-id="132f4-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="132f4-116">**Wszystkie informacje o terminach kalendarza, łącznie z godziną, tematem, lokalizacją i tytułem**</span><span class="sxs-lookup"><span data-stu-id="132f4-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="132f4-117">Kliknij **przycisk zapisz,** aby ustawić reguły zasad udostępniania.</span><span class="sxs-lookup"><span data-stu-id="132f4-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="132f4-118">Jeśli chcesz ustawić te zasady udostępniania jako nowe domyślne zasady udostępniania dla wszystkich użytkowników w organizacji, zaznacz pole wyboru Ustaw te zasady jako domyślne **zasady** udostępniania.</span><span class="sxs-lookup"><span data-stu-id="132f4-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="132f4-119">Kliknij **pozycję zapisz,** aby utworzyć zasady udostępniania.</span><span class="sxs-lookup"><span data-stu-id="132f4-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="132f4-120">**Aby uzyskać pełne zrozumienie tego tematu, przeczytaj:**</span><span class="sxs-lookup"><span data-stu-id="132f4-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="132f4-121">Tworzenie zasad udostępniania w u usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="132f4-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="132f4-122">Stosowanie zasad udostępniania do skrzynek pocztowych w u usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="132f4-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="132f4-123">Modyfikowanie, wyłączanie lub usuwanie zasad udostępniania w u usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="132f4-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)