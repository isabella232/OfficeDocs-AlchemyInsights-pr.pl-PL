---
title: Jak dodawać i zarządzać administratorami — zalecane kroki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678876"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="e6f06-102">Jak dodawać i zarządzać administratorami — zalecane kroki</span><span class="sxs-lookup"><span data-stu-id="e6f06-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="e6f06-103">**Edytuj administratora abonamentu lub współadministratora**</span><span class="sxs-lookup"><span data-stu-id="e6f06-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="e6f06-104">Administrator konta może edytować obie role, a administrator subskrypcji może zmienić tylko współadministratora w [portalu Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="e6f06-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="e6f06-105">Dodawanie lub zmienianie administratorów subskrypcji platformy Azure</span><span class="sxs-lookup"><span data-stu-id="e6f06-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="e6f06-106">**Aktualizowanie subskrypcji subskrypcji lub Co-Administrator dla subskrypcji wewnętrznych (odkupionych)**</span><span class="sxs-lookup"><span data-stu-id="e6f06-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="e6f06-107">Administrator usługi lub współadministrator może samodzielnie obsługiwać tę akcję, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="e6f06-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="e6f06-108">Zaloguj się do [portalu Azure](https://ms.portal.azure.com/#home) , a następnie kliknij pozycję **Zarządzanie kosztami + rozliczenia** w lewym bloku.</span><span class="sxs-lookup"><span data-stu-id="e6f06-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="e6f06-109">Kliknij element wiersza z subskrypcją.</span><span class="sxs-lookup"><span data-stu-id="e6f06-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="e6f06-110">Zostanie otwarty przegląd subskrypcji.</span><span class="sxs-lookup"><span data-stu-id="e6f06-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="e6f06-111">W bloku **subskrypcji** kliknij pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="e6f06-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="e6f06-112">Kliknij przycisk **administrator usługi** .</span><span class="sxs-lookup"><span data-stu-id="e6f06-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="e6f06-113">Wprowadź adres e-mail użytkownika, którego chcesz ustawić jako administratora usługi, i kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="e6f06-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="e6f06-114">**Dodaj/Zmień/Usuń współadministratora**</span><span class="sxs-lookup"><span data-stu-id="e6f06-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="e6f06-115">Zaloguj się w [witrynie Azure Portal](https://ms.portal.azure.com/#home) jako administrator usługi.</span><span class="sxs-lookup"><span data-stu-id="e6f06-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="e6f06-116">Otwórz [abonamenty](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i wybierz abonament.</span><span class="sxs-lookup"><span data-stu-id="e6f06-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="e6f06-117">(Współadministratory mogą być przypisani tylko w zakresie abonamentu).</span><span class="sxs-lookup"><span data-stu-id="e6f06-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="e6f06-118">Przechodzenie do **kontroli dostępu (IAM)**  >  **klasyczny administrator**  >  **Dodaj**  >  opcję **Dodaj współadministratora** , aby otworzyć okienko **Dodaj współadministratora** (Jeśli opcja Dodaj współadministratora jest wyłączona, oznacza to, że nie masz uprawnień).</span><span class="sxs-lookup"><span data-stu-id="e6f06-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="e6f06-119">Wybierz użytkownika, którego chcesz dodać, i kliknij przycisk **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="e6f06-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="e6f06-120">**Dowiedz się więcej:**</span><span class="sxs-lookup"><span data-stu-id="e6f06-120">**Learn more:**</span></span>
- [<span data-ttu-id="e6f06-121">Dodaj współ-administrator</span><span class="sxs-lookup"><span data-stu-id="e6f06-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="e6f06-122">Usuwanie współadministratora</span><span class="sxs-lookup"><span data-stu-id="e6f06-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="e6f06-123">Zmienianie administratora usługi</span><span class="sxs-lookup"><span data-stu-id="e6f06-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="e6f06-124">Wyświetlanie administratora konta</span><span class="sxs-lookup"><span data-stu-id="e6f06-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="e6f06-125">Zarządzanie dostępem przy użyciu funkcji RBAC i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e6f06-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="e6f06-126">**Dodawanie/usuwanie użytkowników przy użyciu usługi Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="e6f06-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="e6f06-127">Możesz dodawać nowych użytkowników lub usuwać istniejących użytkowników z organizacji usługi Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="e6f06-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="e6f06-128">Aby dodać nowego użytkownika, zaloguj się w [witrynie Azure Portal](https://ms.portal.azure.com/#home) jako użytkownik-administrator organizacji.</span><span class="sxs-lookup"><span data-stu-id="e6f06-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="e6f06-129">Wybierz pozycję **Azure Active Directory**, wybierz pozycję **Użytkownicy** , a następnie kliknij pozycję **nowy użytkownik**.</span><span class="sxs-lookup"><span data-stu-id="e6f06-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="e6f06-130">Na stronie **użytkownik** wprowadź wymagane informacje.</span><span class="sxs-lookup"><span data-stu-id="e6f06-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="e6f06-131">Kliknij pozycję **Utwórz**.</span><span class="sxs-lookup"><span data-stu-id="e6f06-131">Click **Create**.</span></span> <span data-ttu-id="e6f06-132">Użytkownik jest tworzony i dodawany do dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6f06-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="e6f06-133">**Dowiedz się więcej**:</span><span class="sxs-lookup"><span data-stu-id="e6f06-133">**Learn more**:</span></span>

- [<span data-ttu-id="e6f06-134">Dodawanie nowego użytkownika</span><span class="sxs-lookup"><span data-stu-id="e6f06-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="e6f06-135">Usuwanie użytkownika</span><span class="sxs-lookup"><span data-stu-id="e6f06-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="e6f06-136">Dodawanie lub aktualizowanie informacji o profilu użytkownika przy użyciu usługi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e6f06-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="e6f06-137">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="e6f06-137">**Recommended documents**</span></span>

- [<span data-ttu-id="e6f06-138">Co to jest kontrola dostępu (RBAC) oparta na rolach?</span><span class="sxs-lookup"><span data-stu-id="e6f06-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="e6f06-139">Opis różnych ról na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="e6f06-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="e6f06-140">Uprawnienia roli administratora w usłudze Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e6f06-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="e6f06-141">Samouczek: udzielanie dostępu użytkownikowi przy użyciu RBAC i usługi Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e6f06-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="e6f06-142">Rozwiązywanie problemów z RBAC na platformie Azure</span><span class="sxs-lookup"><span data-stu-id="e6f06-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="e6f06-143">Organizowanie zasobów za pomocą grup zarządzania platformą Azure</span><span class="sxs-lookup"><span data-stu-id="e6f06-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="e6f06-144">Jak zażądać kopii faktury na platformie Azure za pośrednictwem poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="e6f06-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="e6f06-145">Jak dodawać, aktualizować i usuwać kartę kredytową lub debetową z usługi Azure</span><span class="sxs-lookup"><span data-stu-id="e6f06-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="e6f06-146">Zarządzaj subskrypcją (Aktywuj ponownie/Anuluj/Przełącz)</span><span class="sxs-lookup"><span data-stu-id="e6f06-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



