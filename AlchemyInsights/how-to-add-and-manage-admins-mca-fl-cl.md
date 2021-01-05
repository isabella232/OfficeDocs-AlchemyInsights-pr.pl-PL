---
title: Jak dodawać administratorów i zarządzać nimi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755505"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="841e9-102">Jak dodawać administratorów i zarządzać nimi</span><span class="sxs-lookup"><span data-stu-id="841e9-102">How to add and manage admins</span></span>

<span data-ttu-id="841e9-103">Na podstawie opisu swojego problemu znaleźliśmy rozwiązanie dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="841e9-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="841e9-104">Większość klientów mogła samodzielnie rozwiązać swoje problemy po przeprowadzeniu naszej dokumentacji.</span><span class="sxs-lookup"><span data-stu-id="841e9-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="841e9-105">Aby zarządzać kontem rozliczeniowym na potrzeby umowy z klientami firmy Microsoft (MCA), możesz korzystać z różnych ról z wymaganym poziomem dostępu.</span><span class="sxs-lookup"><span data-stu-id="841e9-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="841e9-106">Role te są uzupełnienieem wbudowanych ról usługi platformy Azure, które ułatwiają sterowanie zasobami.</span><span class="sxs-lookup"><span data-stu-id="841e9-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="841e9-107">**Aby dodać role rozliczeń w portalu Azure:**</span><span class="sxs-lookup"><span data-stu-id="841e9-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="841e9-108">Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="841e9-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="841e9-109">Wyszukaj *Zarządzanie kosztami + rozliczenia*.</span><span class="sxs-lookup"><span data-stu-id="841e9-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="841e9-110">Wybierz pozycję Kontrola dostępu (IAM) w zakresie, na przykład konto rozliczeniowe, profil rozliczeń lub sekcję faktury, w której chcesz udzielić dostępu.</span><span class="sxs-lookup"><span data-stu-id="841e9-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="841e9-111">Na stronie kontrola dostępu (IAM) jest wyświetlana lista użytkowników i grup przypisanych do poszczególnych ról w tym zakresie.</span><span class="sxs-lookup"><span data-stu-id="841e9-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="841e9-112">Aby udzielić dostępu użytkownikowi, wybierz pozycję **Dodaj** od początku strony.</span><span class="sxs-lookup"><span data-stu-id="841e9-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="841e9-113">Z listy rozwijanej *rola* wybierz rolę.</span><span class="sxs-lookup"><span data-stu-id="841e9-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="841e9-114">Wprowadź adres e-mail użytkownika, któremu chcesz udzielić dostępu.</span><span class="sxs-lookup"><span data-stu-id="841e9-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="841e9-115">Wybierz pozycję **Zapisz** , aby przypisać rolę.</span><span class="sxs-lookup"><span data-stu-id="841e9-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="841e9-116">Aby usunąć dostęp użytkownika, zaznacz użytkownika z przypisaną rolą, którą chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="841e9-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="841e9-117">Wybierz pozycję **Usuń**.</span><span class="sxs-lookup"><span data-stu-id="841e9-117">Select **Remove**.</span></span>

<span data-ttu-id="841e9-118">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="841e9-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="841e9-119">Definicje ról rozliczeń</span><span class="sxs-lookup"><span data-stu-id="841e9-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="841e9-120">Zadania i role konta rozliczeniowego</span><span class="sxs-lookup"><span data-stu-id="841e9-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="841e9-121">Rozpoczynanie pracy z kontem rozliczeniowym MCA</span><span class="sxs-lookup"><span data-stu-id="841e9-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="841e9-122">Sprawdzanie dostępu do umowy z klientem firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="841e9-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
