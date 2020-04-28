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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908714"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="e25a2-103">Dzienny limit wiadomości e-mail przekroczony.</span><span class="sxs-lookup"><span data-stu-id="e25a2-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="e25a2-104">Przepływ pracy jest zawieszony.</span><span class="sxs-lookup"><span data-stu-id="e25a2-104">Workflow is suspended.</span></span>

<span data-ttu-id="e25a2-105">Ten błąd może zostać odebrany w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="e25a2-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="e25a2-106">Przepływ pracy w usłudze SharePoint Online jest używany w typie platformy przepływu pracy programu SharePoint 2010 lub SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="e25a2-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="e25a2-107">Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do ponad 200 użytkowników naraz, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="e25a2-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="e25a2-108">Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana i zauważysz następujące zachowanie:</span><span class="sxs-lookup"><span data-stu-id="e25a2-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="e25a2-109">W przypadku przepływu pracy przy użyciu typu platformy programu SharePoint 2013 można przejść do strony **Stan przepływu pracy.**</span><span class="sxs-lookup"><span data-stu-id="e25a2-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="e25a2-110">Na stronie Stan przepływu pracy **stan wewnętrzny** jest ustawiony na **Uruchomiono,** a dymek informacji nie **może wysłać do adresata**.</span><span class="sxs-lookup"><span data-stu-id="e25a2-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="e25a2-111">Aby obejść ten problem, skonfiguruj przepływ pracy tak, aby wysyłał wiadomości e-mail bez [przekraczania limitów nadawców usługi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="e25a2-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="e25a2-112">Na przykład użyj pauzy w przepływie pracy, wyślij wiadomość e-mail do grupy microsoft 365, grupy dystrybucyjnej lub grupy zabezpieczeń z włączoną pocztą lub wyślij wiadomość do mniej niż 200 adresatów naraz.</span><span class="sxs-lookup"><span data-stu-id="e25a2-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="e25a2-113">Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="e25a2-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="e25a2-114">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="e25a2-114">Related topics</span></span>
- [<span data-ttu-id="e25a2-115">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="e25a2-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e25a2-116">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="e25a2-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 