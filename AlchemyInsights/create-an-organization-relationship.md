---
title: Utwórz relację organizacyjną, aby umożliwić użytkownikom współpracę z inną organizacją
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
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816138"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="a9d34-102">Utwórz relację organizacyjną, aby umożliwić użytkownikom współpracę z inną organizacją</span><span class="sxs-lookup"><span data-stu-id="a9d34-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="a9d34-103">Z pulpitu nawigacyjnego centrum administracyjnego platformy Microsoft 365 przejdź do **Administrator** > **Usługa Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a9d34-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="a9d34-104">Przejdź do pozycji **Organizacja** > **Udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="a9d34-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="a9d34-105">W obszarze **Udostępnianie organizacji** kliknij pozycję **Nowe** .</span><span class="sxs-lookup"><span data-stu-id="a9d34-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="a9d34-106">W **nowej relacji organizacji** w polu **Nazwa relacji** wpisz przyjazną nazwę relacji organizacji.</span><span class="sxs-lookup"><span data-stu-id="a9d34-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="a9d34-107">W polu **Domeny do udostępnienia** wpisz domenę dla lokalnej organizacji usługi Office 365 lub usługi Exchange, której chcesz udostępniać kalendarze.</span><span class="sxs-lookup"><span data-stu-id="a9d34-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="a9d34-108">Jeśli chcesz wprowadzić więcej niż jedną domenę, oddziel nazwy domen przecinkami.</span><span class="sxs-lookup"><span data-stu-id="a9d34-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="a9d34-109">Na przykład: contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a9d34-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="a9d34-110">Zaznacz pole wyboru **Włącz udostępnianie informacji o stanie wolny lub zajęty dla kalendarza**, aby włączyć udostępnianie kalendarza w wymienionych domenach.</span><span class="sxs-lookup"><span data-stu-id="a9d34-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="a9d34-111">Ustaw poziom udostępniania informacji wolny lub zajęty dla kalendarza i określ, którzy użytkownicy mogą udostępniać informacje o stanie wolny lub zajęty dla kalendarza.</span><span class="sxs-lookup"><span data-stu-id="a9d34-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="a9d34-112">Aby ustawić poziom dostępu wolny lub zajęty dla kalendarza, wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="a9d34-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="a9d34-113">**Informacje o stanie wolny lub zajęty dla kalendarza zawierające tylko określenie czasu**</span><span class="sxs-lookup"><span data-stu-id="a9d34-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="a9d34-114">**Kalendarz wolny lub zajęty z określeniem czasu, tematu i lokalizacji**</span><span class="sxs-lookup"><span data-stu-id="a9d34-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="a9d34-115">Aby określić, którzy użytkownicy będą udostępniać informacje o stanie wolny lub zajęty dla kalendarza, wybierz jedną z następujących opcji:</span><span class="sxs-lookup"><span data-stu-id="a9d34-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="a9d34-116">**Wszyscy w Twojej organizacji**</span><span class="sxs-lookup"><span data-stu-id="a9d34-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="a9d34-117">**Określona grupa zabezpieczeń**</span><span class="sxs-lookup"><span data-stu-id="a9d34-117">**A specified security group**</span></span>  

<span data-ttu-id="a9d34-118">Kliknij przycisk **Przeglądaj**, aby wybrać grupę zabezpieczeń z listy, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="a9d34-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="a9d34-119">Kliknij przycisk **Zapisz**, aby utworzyć relację organizacyjną.</span><span class="sxs-lookup"><span data-stu-id="a9d34-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="a9d34-120">**Uwaga:** konfiguracje między dzierżawcami nie obsługują kontaktów osobistych na potrzeby wyszukiwania informacji o stanie wolny lub zajęty.</span><span class="sxs-lookup"><span data-stu-id="a9d34-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="a9d34-121">Aby wyszukiwanie informacji o stanie wolny lub zajęty działało, kontakty muszą znajdować się na globalnej liście adresów.</span><span class="sxs-lookup"><span data-stu-id="a9d34-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="a9d34-122">**Aby uzyskać pełne zrozumienie tego tematu, przeczytaj:**</span><span class="sxs-lookup"><span data-stu-id="a9d34-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="a9d34-123">Utwórz relację organizacyjną w usłudze Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a9d34-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="a9d34-124">Zmodyfikuj relację organizacyjną w usłudze Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a9d34-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="a9d34-125">Usuń relację organizacyjną w usłudze Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a9d34-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
