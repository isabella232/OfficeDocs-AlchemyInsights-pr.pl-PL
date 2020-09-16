---
title: Przekroczono dzienny limit poczty e-mail. Przepływ pracy jest wstrzymany.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731573"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="77e9b-103">Przekroczono dzienny limit poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="77e9b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="77e9b-104">Przepływ pracy jest wstrzymany.</span><span class="sxs-lookup"><span data-stu-id="77e9b-104">Workflow is suspended.</span></span>

<span data-ttu-id="77e9b-105">Ten błąd może zostać odebrany w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="77e9b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="77e9b-106">Masz przepływ pracy w usłudze SharePoint Online, w którym jest używany typ platformy przepływ pracy programu SharePoint 2010 lub SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="77e9b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="77e9b-107">W ramach przepływu pracy skonfigurowano wysyłanie niestandardowej wiadomości e-mail do ponad 200 użytkowników jednocześnie, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.</span><span class="sxs-lookup"><span data-stu-id="77e9b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="77e9b-108">Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana, a Użytkownik zauważy następujące zachowanie:</span><span class="sxs-lookup"><span data-stu-id="77e9b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="77e9b-109">W przypadku przepływu pracy korzystającego z typu platformy programu SharePoint 2013 przejdź do strony **stan przepływu pracy** .</span><span class="sxs-lookup"><span data-stu-id="77e9b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="77e9b-110">Na stronie stan przepływu pracy jest ustawiany **stan wewnętrzny** **, a**w dymku informacji jest wyświetlany komunikat **nie można wysłać do adresata**.</span><span class="sxs-lookup"><span data-stu-id="77e9b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="77e9b-111">Aby obejść ten problem, skonfiguruj przepływ pracy w celu wysyłania wiadomości e-mail bez przekroczenia [limitów nadawcy usługi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="77e9b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="77e9b-112">Na przykład w przepływie pracy można użyć funkcji wstrzymania, wysłać wiadomość e-mail 365 do grupy dystrybucyjnej, grupy dystrybucyjnej lub grupy zabezpieczeń z obsługą poczty albo wysłać wiadomość do mniej niż 200 adresatów jednocześnie.</span><span class="sxs-lookup"><span data-stu-id="77e9b-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="77e9b-113">Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="77e9b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="77e9b-114">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="77e9b-114">Related topics</span></span>
- [<span data-ttu-id="77e9b-115">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="77e9b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="77e9b-116">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="77e9b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 