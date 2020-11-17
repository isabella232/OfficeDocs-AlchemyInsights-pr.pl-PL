---
title: Uprzywilejowana rola zarządzania tożsamością
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088877"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="5cf9e-102">Rola uprzywilejowanego zarządzania tożsamościami (PIM)</span><span class="sxs-lookup"><span data-stu-id="5cf9e-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="5cf9e-103">**Uprawnienia nie są udzielane po aktywowaniu roli**</span><span class="sxs-lookup"><span data-stu-id="5cf9e-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="5cf9e-104">Po aktywowaniu roli w usłudze Azure AD o uprzywilejowanym zarządzaniu tożsamości (PIM) Aktywacja może nie zostać natychmiast rozpropagowana do wszystkich portali wymagających roli uprzywilejowanej.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="5cf9e-105">Czasami nawet w przypadku propagacji zmiany buforowanie w sieci Web w portalu może spowodować, że zmiana nie zostanie wprowadzona od razu.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="5cf9e-106">Jeśli aktywacja jest opóźniona, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="5cf9e-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5cf9e-107">Wyloguj się z portalu Azure, a następnie zaloguj się ponownie.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="5cf9e-108">Po aktywowaniu roli usługi Azure AD lub roli zasobów platformy Azure zostaną wyświetlone etapy aktywacji.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="5cf9e-109">Po zakończeniu wszystkich etapów zostanie wyświetlone łącze Wyloguj.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="5cf9e-110">Możesz użyć tego linku, aby się wylogować. Spowoduje to rozwiązanie większości przypadków opóźnienia aktywacji.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="5cf9e-111">W programie PIM Sprawdź, czy jesteś członkiem roli.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="5cf9e-112">Jeśli uaktywniasz rolę administratora programu Exchange, upewnij się, że wylogowano się i zaloguj się ponownie.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="5cf9e-113">Jeśli problem będzie nadal występował, Otwórz bilet pomocy technicznej i zwiększ go jako problem.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="5cf9e-114">Jeśli korzystasz z roli administratora programu Exchange, aby uzyskać dostęp do centrum zabezpieczeń i zgodności, zobacz następny krok.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="5cf9e-115">Jeśli uaktywniasz rolę w celu uzyskania dostępu do centrum zabezpieczeń i zgodności albo jeśli uaktywniasz rolę administratora programu SharePoint, będziesz mieć pewne opóźnienie aktywacji od kilku minut do kilku godzin.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="5cf9e-116">Jest to znany problem i aktywnie pracujemy nad tym zespołem w celu możliwie jak najszybszego rozwiązania problemu.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="5cf9e-117">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="5cf9e-117">For more information, see:</span></span>

- [<span data-ttu-id="5cf9e-118">Aktywowanie ról usługi Azure AD w programie PIM</span><span class="sxs-lookup"><span data-stu-id="5cf9e-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="5cf9e-119">Aktywowanie ról zasobów platformy Azure w programie PIM</span><span class="sxs-lookup"><span data-stu-id="5cf9e-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="5cf9e-120">**Uprawnienia nie są usuwane po zdezaktywowaniu roli lub wygaśnięciu aktywacji roli**</span><span class="sxs-lookup"><span data-stu-id="5cf9e-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="5cf9e-121">Po zdezaktywowaniu roli w ramach uprzywilejowanego zarządzania tożsamościami usługi Azure AD lub po wygaśnięciu okresu aktywacji roli może istnieć opóźnienie, w którym nadal masz dostęp.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="5cf9e-122">Jeśli dezaktywacja jest opóźniona, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="5cf9e-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5cf9e-123">Jeśli użytkownik dezaktywuje rolę administratora programu Exchange lub upłynie okres aktywacji roli, a Użytkownik zauważy znaczne opóźnienie przed usunięciem uprawnień, należy otworzyć bilet pomocy technicznej i poinstruować inżyniera pomocy technicznej, aby pomóc Ci w zalogowaniu się do biletu za pomocą zespołu PAM (uprzywilejowanego zarządzania dostępem) w pakiecie Office o tym problemie.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="5cf9e-124">Jeśli okres aktywacji upłynął, ale nadal masz otwartą sesję przeglądarki, zamknij przeglądarkę.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="5cf9e-125">Możesz nadal korzystać z tej roli, dopóki nie zamkniesz tej sesji.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="5cf9e-126">Jest to znany problem, który umożliwia jednoczesne cofnięcie każdej sesji po wygaśnięciu aktywacji.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="5cf9e-127">Jeśli opóźnienie różni się od tych dwóch scenariuszy, należy otworzyć bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="5cf9e-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
