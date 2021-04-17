---
title: Migracja z usługi AIP do rozwiązania MIP/unified Labeling w Centrum zgodności
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825381"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="a7794-102">Migracja z usługi AIP do rozwiązania MIP/unified Labeling w Centrum zgodności</span><span class="sxs-lookup"><span data-stu-id="a7794-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="a7794-103">Aby przeprowadzić migrację etykiet AIP do funkcji Unified Labeling w Centrum zabezpieczeń i zgodności, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a7794-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="a7794-104">**Aktywowanie ochrony z portalu Azure Portal**</span><span class="sxs-lookup"><span data-stu-id="a7794-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="a7794-105">Jeśli jeszcze tego nie zrobiono, otwórz nowe okno przeglądarki i [zaloguj się do portalu Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="a7794-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="a7794-106">Przejdź do **bladej usługi Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="a7794-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="a7794-107">Na przykład w menu Centrum kliknij pozycję **Wszystkie** usługi i zacznij wpisywać **informacje** w polu Filtruj.</span><span class="sxs-lookup"><span data-stu-id="a7794-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="a7794-108">Wybierz **pozycję Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="a7794-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="a7794-109">Jeśli do tej pory nie uzyskiwano dostępu do grota usługi Azure Information Protection, zapoznaj się z dodatkowymi czynnościami w celu dodania tego grota do portalu. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)</span><span class="sxs-lookup"><span data-stu-id="a7794-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="a7794-110">Aby otworzyć blok danych usługi Azure Information Protection, musisz mieć [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) lub plan usługi Office 365, który obejmuje zarządzanie prawami.</span><span class="sxs-lookup"><span data-stu-id="a7794-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="a7794-111">Jeśli masz jedną z tych subskrypcji, ale jest wyświetlany komunikat informujący, że nie można odnaleźć ważnej subskrypcji, skontaktuj się z pomocą techniczną firmy [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) lub skorzystaj ze standardowych kanałów pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="a7794-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="a7794-112">Znajdź opcje menu **Zarządzaj** i wybierz pozycję **Aktywacja ochrony.**</span><span class="sxs-lookup"><span data-stu-id="a7794-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="a7794-113">Kliknij **przycisk** Aktywuj , a następnie potwierdź swoje działanie.</span><span class="sxs-lookup"><span data-stu-id="a7794-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="a7794-114">Po zakończeniu aktywacji na pasku informacji zostanie wyświetlony **komunikat Pomyślnie ukończono aktywację.**</span><span class="sxs-lookup"><span data-stu-id="a7794-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="a7794-115">**Migrowanie etykiet usługi Azure Information Protection do Centrum zabezpieczeń & Office 365**</span><span class="sxs-lookup"><span data-stu-id="a7794-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="a7794-116">Upewnij się, że zalogowano się jako użytkownik z uprawnieniami administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="a7794-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="a7794-117">Przejdź do **bladej usługi Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="a7794-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="a7794-118">Z menu **Zarządzaj** wybierz pozycję **Ujednolicone etykiety**.</span><span class="sxs-lookup"><span data-stu-id="a7794-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="a7794-119">Na stronie **Azure Information Protection — ujednolicone pole etykiet** kliknij przycisk **Aktywuj** i postępuj zgodnie z instrukcjami online.</span><span class="sxs-lookup"><span data-stu-id="a7794-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="a7794-120">**Uwaga:** przed aktywowaniem migracji Centrum zgodności w centrum zabezpieczeń & upewnij się, że masz odpowiednie uprawnienia.</span><span class="sxs-lookup"><span data-stu-id="a7794-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="a7794-121">Aby uzyskać więcej informacji, zobacz następujące artykuły:</span><span class="sxs-lookup"><span data-stu-id="a7794-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="a7794-122">Czy musisz być administratorem globalnym, aby skonfigurować usługę Azure Information Protection, czy mogę delegować innych administratorów?</span><span class="sxs-lookup"><span data-stu-id="a7794-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="a7794-123">Ważne informacje o rolach administracyjnych po migracji do Centrum & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="a7794-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="a7794-124">Aby uzyskać więcej informacji na temat migracji Z usługi AIP do usługi Unified Labeling do Centrum zabezpieczeń i zgodności, zobacz [Migrowanie etykiet.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="a7794-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
