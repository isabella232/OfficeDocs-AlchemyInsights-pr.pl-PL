---
title: Migracja z centrali Środkowej do MCI/ujednolicona etykietowanie w centrum zgodności
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674336"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="6275d-102">Migracja z centrali Środkowej do MCI/ujednolicona etykietowanie w centrum zgodności</span><span class="sxs-lookup"><span data-stu-id="6275d-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="6275d-103">Aby przeprowadzić migrację z etykiet centralnych do ujednoliconych etykiet w centrum zabezpieczeń i zgodności, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="6275d-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="6275d-104">**Aktywowanie ochrony w portalu Azure**</span><span class="sxs-lookup"><span data-stu-id="6275d-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="6275d-105">Jeśli jeszcze tego nie zrobiono, Otwórz nowe okno przeglądarki i [Zaloguj się w witrynie Azure Portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="6275d-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="6275d-106">Przejdź do bloku **Ochrona informacji platformy Azure** .</span><span class="sxs-lookup"><span data-stu-id="6275d-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="6275d-107">Na przykład w menu centrum kliknij pozycję **wszystkie usługi** i zacznij wpisywać **informacje** w polu Filtr.</span><span class="sxs-lookup"><span data-stu-id="6275d-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="6275d-108">Wybierz pozycję **Ochrona informacji platformy Azure**.</span><span class="sxs-lookup"><span data-stu-id="6275d-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="6275d-109">Jeśli nie uzyskano dostępu do bloku usługi Azure Information Protection, zobacz [dodatkowe czynności](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , które umożliwiają dodanie tego bloku do portalu.</span><span class="sxs-lookup"><span data-stu-id="6275d-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="6275d-110">Aby otworzyć blok usługi Azure Information Protection, musisz mieć [Plan Premium (Azure Information Protection](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ) lub plan Office 365, który zawiera Zarządzanie prawami.</span><span class="sxs-lookup"><span data-stu-id="6275d-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="6275d-111">Jeśli masz już taką subskrypcję, ale widzisz komunikat, że nie można znaleźć prawidłowego abonamentu, [skontaktuj się z pomocą techniczną firmy Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) lub skorzystaj ze standardowych kanałów pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="6275d-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="6275d-112">Znajdź opcje menu **Zarządzaj** , a następnie wybierz pozycję **Aktywacja ochrony**.</span><span class="sxs-lookup"><span data-stu-id="6275d-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="6275d-113">Kliknij pozycję **Aktywuj**, a następnie Potwierdź działanie.</span><span class="sxs-lookup"><span data-stu-id="6275d-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="6275d-114">Po zakończeniu aktywacji na pasku informacji jest wyświetlana informacja, że **Aktywacja została pomyślnie zakończona**.</span><span class="sxs-lookup"><span data-stu-id="6275d-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="6275d-115">**Migrowanie etykiet ochrony informacji platformy Azure do usługi Office 365 Security & Centrum zgodności**</span><span class="sxs-lookup"><span data-stu-id="6275d-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="6275d-116">Upewnij się, że zalogowano się jako użytkownik z uprawnieniami administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="6275d-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="6275d-117">Przejdź do bloku **Ochrona informacji platformy Azure** .</span><span class="sxs-lookup"><span data-stu-id="6275d-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="6275d-118">W menu **Zarządzaj** wybierz opcję **ujednolicone etykietowanie**.</span><span class="sxs-lookup"><span data-stu-id="6275d-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="6275d-119">Na **wbudowanym bloku etykiet na platformie Azure Information Protection** kliknij pozycję **Aktywuj** i postępuj zgodnie z instrukcjami online.</span><span class="sxs-lookup"><span data-stu-id="6275d-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="6275d-120">**Uwaga**: Sprawdź, czy masz odpowiednie uprawnienia, zanim uaktywnisz migrację centrum zabezpieczeń & zgodności.</span><span class="sxs-lookup"><span data-stu-id="6275d-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="6275d-121">Aby uzyskać więcej informacji, zobacz następujące artykuły:</span><span class="sxs-lookup"><span data-stu-id="6275d-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="6275d-122">Czy musisz być administratorem globalnym w celu skonfigurowania usługi Azure Information Protection lub można delegować do innych administratorów?</span><span class="sxs-lookup"><span data-stu-id="6275d-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="6275d-123">Ważne informacje dotyczące ról administracyjnych po przeprowadzeniu migracji do centrum zgodności z zabezpieczeniami &.</span><span class="sxs-lookup"><span data-stu-id="6275d-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="6275d-124">Aby uzyskać więcej informacji na temat podwyższania poziomu migracji etykiet do centrum zabezpieczeń i zgodności, zobacz [Migrowanie etykiet](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="6275d-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
