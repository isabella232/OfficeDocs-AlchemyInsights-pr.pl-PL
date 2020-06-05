---
title: Przekroczono dzienny limit wiadomości e-mail. Przepływ pracy jest zawieszony.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580343"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="1efdf-103">Dzienny limit wiadomości e-mail przekroczony.</span><span class="sxs-lookup"><span data-stu-id="1efdf-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="1efdf-104">Przepływ pracy jest zawieszony.</span><span class="sxs-lookup"><span data-stu-id="1efdf-104">Workflow is suspended.</span></span>

<span data-ttu-id="1efdf-105">Ten błąd może zostać odebrany w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="1efdf-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="1efdf-106">Przepływ pracy w usłudze SharePoint Online jest używany w typie platformy przepływu pracy programu SharePoint 2010 lub SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="1efdf-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="1efdf-107">Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do ponad 200 użytkowników naraz, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="1efdf-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="1efdf-108">Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana i zauważysz następujące zachowanie:</span><span class="sxs-lookup"><span data-stu-id="1efdf-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="1efdf-109">W przypadku przepływu pracy przy użyciu typu platformy programu SharePoint 2013 można przejść do strony **Stan przepływu pracy.**</span><span class="sxs-lookup"><span data-stu-id="1efdf-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="1efdf-110">Na stronie Stan przepływu pracy **stan wewnętrzny** jest ustawiony na **Uruchomiono,** a dymek informacji nie **może wysłać do adresata**.</span><span class="sxs-lookup"><span data-stu-id="1efdf-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="1efdf-111">Aby obejść ten problem, skonfiguruj przepływ pracy tak, aby wysyłał wiadomości e-mail bez [przekraczania limitów nadawców usługi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="1efdf-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="1efdf-112">Na przykład użyj pauzy w przepływie pracy, wyślij wiadomość e-mail do grupy microsoft 365, grupy dystrybucyjnej lub grupy zabezpieczeń z włączoną pocztą lub wyślij wiadomość do mniej niż 200 adresatów naraz.</span><span class="sxs-lookup"><span data-stu-id="1efdf-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="1efdf-113">Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="1efdf-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="1efdf-114">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="1efdf-114">Related topics</span></span>
- [<span data-ttu-id="1efdf-115">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="1efdf-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1efdf-116">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="1efdf-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 