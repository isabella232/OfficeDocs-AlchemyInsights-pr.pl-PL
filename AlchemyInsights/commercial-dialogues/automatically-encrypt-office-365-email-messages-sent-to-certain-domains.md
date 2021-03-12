---
title: Automatyczne szyfrowanie wiadomości e-mail usługi Office 365 wysyłanych do określonych domen
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749305"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="ffbcf-102">Automatyczne szyfrowanie wiadomości e-mail usługi Office 365 wysyłanych do określonych domen</span><span class="sxs-lookup"><span data-stu-id="ffbcf-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="ffbcf-103">W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz pozycję **przepływ poczty > reguły**.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="ffbcf-104">Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości i ochronę praw do wiadomości w usłudze **Office 365.**</span><span class="sxs-lookup"><span data-stu-id="ffbcf-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="ffbcf-105">W **imieniu** użytkownika wprowadź nazwę reguły, na przykład Szyfruj *wiadomości wysyłane do contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="ffbcf-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="ffbcf-106">W **edycie Zastosuj tę regułę, jeśli** wybierz pozycję **> domeną jest**.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="ffbcf-107">Wprowadź nazwę domeny, na przykład **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="ffbcf-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="ffbcf-108">Kliknij **ikonę Dodaj (+),** a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="ffbcf-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="ffbcf-109">Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="ffbcf-110">W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="ffbcf-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="ffbcf-111">(Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="ffbcf-112">Ale możesz je dodać!)</span><span class="sxs-lookup"><span data-stu-id="ffbcf-112">But you can add it!)</span></span>
9. <span data-ttu-id="ffbcf-113">Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).</span><span class="sxs-lookup"><span data-stu-id="ffbcf-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="ffbcf-114">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ffbcf-115">Zawsze możesz wrócić i edytować tę regułę później.</span><span class="sxs-lookup"><span data-stu-id="ffbcf-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="ffbcf-116">Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty w celu szyfrowania wiadomości e-mail [w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="ffbcf-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>