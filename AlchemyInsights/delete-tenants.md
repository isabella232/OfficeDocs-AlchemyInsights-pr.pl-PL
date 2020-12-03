---
title: Usuwanie dzierżawy
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564885"
---
# <a name="delete-tenant"></a><span data-ttu-id="a550d-102">Usuwanie dzierżawy</span><span class="sxs-lookup"><span data-stu-id="a550d-102">Delete tenant</span></span>

<span data-ttu-id="a550d-103">Aby usunąć usługę Azure AD, upewnij się, że:</span><span class="sxs-lookup"><span data-stu-id="a550d-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="a550d-104">Jesteś administratorem globalnym w katalogu.</span><span class="sxs-lookup"><span data-stu-id="a550d-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="a550d-105">Użytkownik nie jest zalogowany przy użyciu konta, które ma katalog domyślny, taki jak contoso.onmicrosoft.com na koncie zalogowanym, na przykład admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="a550d-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="a550d-106">Przed usunięciem Usuń wszystkie aktywne aplikacje w katalogu.</span><span class="sxs-lookup"><span data-stu-id="a550d-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="a550d-107">Aby usunąć aktywne aplikacje, przejdź do rejestracji aplikacji i Usuń istniejące aplikacje.</span><span class="sxs-lookup"><span data-stu-id="a550d-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="a550d-108">Nie ma aktywnych subskrypcji żadnych usług Microsoft Online, takich jak Microsoft Azure, Office 365 lub Azure AD Premium, które są skojarzone z katalogiem.</span><span class="sxs-lookup"><span data-stu-id="a550d-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="a550d-109">Przekazywanie abonamentów lub przyspieszanie anulowania aktywnych subskrypcji za pośrednictwem usługi Azure support i rozliczenia.</span><span class="sxs-lookup"><span data-stu-id="a550d-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="a550d-110">Dowiedz się więcej o tym, jak anulować subskrypcję usługi Office 365 i subskrypcje platformy Azure.</span><span class="sxs-lookup"><span data-stu-id="a550d-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="a550d-111">Aby uzyskać wskazówki dotyczące kojarzenia lub dodawania istniejącej subskrypcji do dzierżawy, zobacz [kojarzenie lub Dodawanie subskrypcji platformy Azure do dzierżawy usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="a550d-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="a550d-112">Brak aktywnych licencji.</span><span class="sxs-lookup"><span data-stu-id="a550d-112">There are no Active license.</span></span> <span data-ttu-id="a550d-113">Aby usunąć licencje, zobacz [Jak usunąć subskrypcję w celu usunięcia licencji](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="a550d-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="a550d-114">Po próbie usunięcia usługi Azure AD nie ma żadnych innych aktywnych użytkowników w katalogu, ani jako Administrator globalny.</span><span class="sxs-lookup"><span data-stu-id="a550d-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="a550d-115">Usuń wszystkich innych aktywnych użytkowników, a wszystkie zależności dotyczące niestandardowej nazwy domeny w dzierżawie również muszą zostać usunięte, na przykład użytkownicy utworzeni za pomocą admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a550d-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="a550d-116">Aby uzyskać więcej szczegółowych informacji na temat następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="a550d-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="a550d-117">Usuń usługę Azure Active Directory lub "abonament", zobacz [usuwanie usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="a550d-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="a550d-118">Usuwanie aplikacji w katalogu, zobacz [usuwanie aplikacji](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="a550d-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
