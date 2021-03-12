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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749440"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="9eb24-102">Automatyczne szyfrowanie niektórych wiadomości e-mail usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="9eb24-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="9eb24-103">Wiadomości wysyłane przez użytkowników do określonych osób zewnętrznych lub organizacji mogą być automatycznie szyfrowane.</span><span class="sxs-lookup"><span data-stu-id="9eb24-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="9eb24-104">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="9eb24-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="9eb24-105">W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz pozycję **przepływ poczty > reguły**.</span><span class="sxs-lookup"><span data-stu-id="9eb24-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9eb24-106">Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości i ochronę praw do wiadomości w usłudze **Office 365.**</span><span class="sxs-lookup"><span data-stu-id="9eb24-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9eb24-107">W **imieniu** użytkownika wprowadź nazwę reguły, na przykład Szyfruj *wiadomości wysyłane do DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="9eb24-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="9eb24-108">W **edycie Zastosuj tę regułę, jeśli** wybierz pozycję **Adresatem > jest ta osoba**.</span><span class="sxs-lookup"><span data-stu-id="9eb24-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="9eb24-109">W **oknie Wybieranie** członków wybierz imię i nazwisko osoby, której chcesz użyć reguły szyfrowania, a następnie kliknij pozycję **dodaj**.</span><span class="sxs-lookup"><span data-stu-id="9eb24-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="9eb24-110">Po dodaniu użytkowników kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="9eb24-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="9eb24-111">Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**.</span><span class="sxs-lookup"><span data-stu-id="9eb24-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="9eb24-112">W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="9eb24-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9eb24-113">(Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="9eb24-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9eb24-114">Ale możesz je dodać!)</span><span class="sxs-lookup"><span data-stu-id="9eb24-114">But you can add it!)</span></span>
9. <span data-ttu-id="9eb24-115">Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).</span><span class="sxs-lookup"><span data-stu-id="9eb24-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9eb24-116">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9eb24-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9eb24-117">Zawsze możesz wrócić i edytować tę regułę później.</span><span class="sxs-lookup"><span data-stu-id="9eb24-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9eb24-118">Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty e-mail w celu szyfrowania wiadomości e-mail [w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="9eb24-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

