---
title: Przekroczono dzienny limit wiadomości e-mail. Przepływ pracy jest zawieszone.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059648"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a3fe5-103">Przekroczony Limit dzienny poczta elektroniczna.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a3fe5-104">Przepływ pracy jest zawieszone.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-104">Workflow is suspended.</span></span>

<span data-ttu-id="a3fe5-105">Tego błędu mogą pojawić się w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="a3fe5-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a3fe5-106">Masz przepływu pracy programu SharePoint Online używanego programu SharePoint 2010 lub typ platformy przepływu pracy programu SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a3fe5-107">Przepływ pracy jest skonfigurowany do wysyłania wiadomości e-mail niestandardowych do więcej niż 200 użytkowników w czasie, więcej niż 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a3fe5-108">Po uruchomieniu przepływu pracy nie jest wysyłana wiadomość e-mail, a można zauważyć następujące zachowanie:</span><span class="sxs-lookup"><span data-stu-id="a3fe5-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a3fe5-109">Dla przepływu pracy przy użyciu typu platformy SharePoint 2013 przejdź do strony **Stan przepływu pracy** .</span><span class="sxs-lookup"><span data-stu-id="a3fe5-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a3fe5-110">Na stronie Stan przepływu pracy **Wewnętrzny stan** jest ustawiony na **Rozpoczęte**i wyświetla dymek informacyjny **nie można wysłać do adresata**.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a3fe5-111">Aby obejść ten problem, należy skonfigurować przepływu pracy do wysyłania wiadomości e-mail bez przekroczenia [limitów nadawcy programu Exchange w trybie Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a3fe5-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a3fe5-112">Na przykład za pomocą pause w przepływie pracy, Wyślij wiadomość e-mail do grupy usługi Office 365, grupy dystrybucyjnej lub grupy zabezpieczeń włączoną obsługę poczty lub wysłać wiadomość do mniej niż 200 adresatów naraz.</span><span class="sxs-lookup"><span data-stu-id="a3fe5-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a3fe5-113">Aby uzyskać więcej informacji zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a3fe5-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a3fe5-114">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="a3fe5-114">Related topics</span></span>
- [<span data-ttu-id="a3fe5-115">Utworzyć przepływ</span><span class="sxs-lookup"><span data-stu-id="a3fe5-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a3fe5-116">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="a3fe5-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 