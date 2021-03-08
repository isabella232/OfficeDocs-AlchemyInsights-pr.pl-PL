---
title: Automatyczne szyfrowanie niektórych wiadomości e-mail z usługi Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526759"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="d0bb5-102">Automatyczne szyfrowanie niektórych wiadomości e-mail z usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="d0bb5-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="d0bb5-103">W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz przepływ **poczty e-mail > reguły.**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="d0bb5-104">Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości usługi **Office 365** i ochronę praw do wiadomości.</span><span class="sxs-lookup"><span data-stu-id="d0bb5-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="d0bb5-105">W **nazwie** wprowadź nazwę reguły, na przykład *Zaszyfruj wszystkie wiadomości.*</span><span class="sxs-lookup"><span data-stu-id="d0bb5-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="d0bb5-106">W **przycisku Zastosuj tę regułę, jeśli** wybierz **pozycję [Zastosuj do wszystkich wiadomości]**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="d0bb5-107">Obok pola **Wykonaj następujące czynności** kliknij pozycję **Wybierz.**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="d0bb5-108">W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj,** a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="d0bb5-109">(Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="d0bb5-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="d0bb5-110">Ale możesz go dodać!)</span><span class="sxs-lookup"><span data-stu-id="d0bb5-110">But you can add it!)</span></span>
7. <span data-ttu-id="d0bb5-111">Zaznacz pole **wyboru Inspekcja tej reguły z poziomem** ważności, a następnie wybierz odpowiedni poziom.</span><span class="sxs-lookup"><span data-stu-id="d0bb5-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="d0bb5-112">Jeśli Twoja firma ma zobowiązania kontraktowe dotyczące wysyłania wszystkich zaszyfrowanych wiadomości e-mail, zalecam ustawienie poziomu **Wysoki.**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="d0bb5-113">W **obszarze Wybierz model dla tej reguły** kliknij pozycję **Wymuszaj.**</span><span class="sxs-lookup"><span data-stu-id="d0bb5-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="d0bb5-114">Wybierz dowolną opcję opcjonalną (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele można zostawić przy ustawieniu domyślnym dla prostoty).</span><span class="sxs-lookup"><span data-stu-id="d0bb5-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="d0bb5-115">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="d0bb5-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d0bb5-116">Zawsze możesz wrócić i edytować tę regułę później.</span><span class="sxs-lookup"><span data-stu-id="d0bb5-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="d0bb5-117">Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty e-mail w celu szyfrowania wiadomości e-mail [w usłudze Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="d0bb5-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

