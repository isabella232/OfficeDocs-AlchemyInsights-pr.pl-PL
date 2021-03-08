---
title: Automatyczne szyfrowanie niektórych wiadomości e-mail usługi Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526737"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="70eeb-102">Automatyczne szyfrowanie niektórych wiadomości e-mail w usłudze Office 365</span><span class="sxs-lookup"><span data-stu-id="70eeb-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="70eeb-103">Możesz automatycznie szyfrować wiadomości wysyłane przez użytkowników do określonych osób zewnętrznych lub organizacji.</span><span class="sxs-lookup"><span data-stu-id="70eeb-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="70eeb-104">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="70eeb-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="70eeb-105">W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz przepływ **poczty e-mail > reguły.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="70eeb-106">Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości usługi **Office 365** i ochronę praw do wiadomości.</span><span class="sxs-lookup"><span data-stu-id="70eeb-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="70eeb-107">W **nazwie** wprowadź nazwę reguły, na przykład Szyfrowanie wiadomości *wysyłanych* do DrToniRamos@gmail.com.</span><span class="sxs-lookup"><span data-stu-id="70eeb-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="70eeb-108">W **opcji Zastosuj tę regułę, jeśli** wybierz pozycję **Adresatem > jest ta osoba.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="70eeb-109">W **oknie Wybieranie** członków wybierz imię i nazwisko osoby, do której chcesz zastosować regułę szyfrowania, a następnie kliknij przycisk **Dodaj.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="70eeb-110">Po dodaniu użytkowników kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="70eeb-111">Obok pola **Wykonaj następujące czynności** kliknij pozycję **Wybierz.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="70eeb-112">W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj,** a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="70eeb-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="70eeb-113">(Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="70eeb-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="70eeb-114">Ale możesz go dodać!)</span><span class="sxs-lookup"><span data-stu-id="70eeb-114">But you can add it!)</span></span>
9. <span data-ttu-id="70eeb-115">Wybierz dowolną opcję opcjonalną (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele można zostawić przy ustawieniu domyślnym dla prostoty).</span><span class="sxs-lookup"><span data-stu-id="70eeb-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="70eeb-116">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="70eeb-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="70eeb-117">Zawsze możesz wrócić i edytować tę regułę później.</span><span class="sxs-lookup"><span data-stu-id="70eeb-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="70eeb-118">Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty e-mail w celu szyfrowania wiadomości [e-mail w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="70eeb-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

