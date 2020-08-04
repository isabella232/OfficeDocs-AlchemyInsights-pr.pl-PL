---
title: Problemy z korzystaniem z konsoli administracyjnej usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555388"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="f464f-102">Problemy z korzystaniem z konsoli administracyjnej usługi Intune</span><span class="sxs-lookup"><span data-stu-id="f464f-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="f464f-103">**"Odmowa dostępu" podczas nawigacji po portalu administracyjnym usługi Intune.**</span><span class="sxs-lookup"><span data-stu-id="f464f-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="f464f-104">Jeśli jesteś członkiem roli niestandardowej usługi Intune, upewnij się, że do Twojego konta jest przypisana licencja usługi Intune lub Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="f464f-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="f464f-105">Jeśli do zarządzania urządzeniami używasz programu Menedżer konfiguracji, sprawdź, czy nie należysz do kolekcji użytkowników usługi Intune dla programu MDM programu Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f464f-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="f464f-106">Sprawdź, czy w bloku role usługi Intune przypisano odpowiednie uprawnienia kontroli administracji opartej na rolach (RBAC).</span><span class="sxs-lookup"><span data-stu-id="f464f-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="f464f-107">Sprawdź, czy używana grupa nie jest listą dystrybucyjną.</span><span class="sxs-lookup"><span data-stu-id="f464f-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="f464f-108">Usługa Intune w portalu Azure obsługuje tylko konta użytkowników należących do grup zabezpieczeń usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f464f-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="f464f-109">Przejrzyj swoje grupy w witrynie Azure portal > grupy **usługi Intune**  >  **Groups**lub w witrynie Azure portal > usługi Azure **Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="f464f-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="f464f-110">**Użytkownik ma zbyt wiele uprawnień dla przypisanej roli usługi Intune**</span><span class="sxs-lookup"><span data-stu-id="f464f-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="f464f-111">Należy zaradzić użytkownikowi, aby przejść do ról **usługi**  >  **Intune Usługi Intune**  >  **Moje uprawnienia**  >  **Eksportuj** do przeglądu przyznanych uprawnień.</span><span class="sxs-lookup"><span data-stu-id="f464f-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="f464f-112">**Dodałem grupę zakresu do roli, ale użytkownicy w tej roli nadal widzą innych użytkowników lub urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="f464f-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="f464f-113">Grupy zakresów nie odfiltrowują użytkowników ani urządzeń.</span><span class="sxs-lookup"><span data-stu-id="f464f-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="f464f-114">Grupy zakresów:</span><span class="sxs-lookup"><span data-stu-id="f464f-114">Scope groups:</span></span>

- <span data-ttu-id="f464f-115">Ogranicz, do kogo użytkownicy mogą przypisywać zasady lub aplikacje.</span><span class="sxs-lookup"><span data-stu-id="f464f-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="f464f-116">Zezwalaj tylko określonym użytkownikom na uruchamianie zadań zdalnych na urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="f464f-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="f464f-117">Aby uzyskać więcej informacji na temat grup zakresów, zobacz [Kontrola dostępu oparta na rolach (RBAC) w usłudze Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="f464f-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="f464f-118">**Dodałem użytkownika do roli usługi Intune, ale nadal ma on pełny dostęp do konsoli administracyjnej usługi Intune.**</span><span class="sxs-lookup"><span data-stu-id="f464f-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="f464f-119">Przejdź do usługi Intune > **użytkownicy** w witrynie Azure portal i sprawdź, czy użytkownik nie jest przypisany do żadnej z następujących ról w witrynie Azure portal:</span><span class="sxs-lookup"><span data-stu-id="f464f-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="f464f-120">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="f464f-120">Global administrator</span></span>
- <span data-ttu-id="f464f-121">Administrator usługi usługi Intune</span><span class="sxs-lookup"><span data-stu-id="f464f-121">Intune service administrator</span></span>
- <span data-ttu-id="f464f-122">Administrator usługi SharePoint</span><span class="sxs-lookup"><span data-stu-id="f464f-122">SharePoint administrator</span></span>

<span data-ttu-id="f464f-123">Aby uzyskać więcej informacji, zobacz [Kontrola dostępu oparta na rolach (RBAC) w usłudze Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="f464f-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="f464f-124">**Problemy z dostępem**</span><span class="sxs-lookup"><span data-stu-id="f464f-124">**Access Issues**</span></span>

<span data-ttu-id="f464f-125">Aby uzyskać więcej informacji, zobacz [Nie można zalogować się do usługi Office 365, platformy Azure ani usługi Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="f464f-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>