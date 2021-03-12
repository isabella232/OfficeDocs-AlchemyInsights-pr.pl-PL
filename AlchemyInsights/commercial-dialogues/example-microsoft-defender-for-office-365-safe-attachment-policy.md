---
title: Przykład zasad bezpiecznego załącznika w usłudze Microsoft Defender dla usługi Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749201"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="e6cd1-102">Przykład zasad bezpiecznego załącznika w usłudze Microsoft Defender dla usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="e6cd1-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="e6cd1-103">Te ustawienia umożliwiają obsługę zasad o nazwie *Bez* opóźnień, która natychmiast dostarcza wiadomości, a następnie ponownie podłącza załączniki po ich zeskanowaniu:</span><span class="sxs-lookup"><span data-stu-id="e6cd1-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="e6cd1-104">**Nazwa:** Brak opóźnień</span><span class="sxs-lookup"><span data-stu-id="e6cd1-104">**Name**: No delays</span></span>
- <span data-ttu-id="e6cd1-105">**Opis:** Natychmiast dostarcza wiadomości i ponownie podłącza załączniki po zeskanowaniu.</span><span class="sxs-lookup"><span data-stu-id="e6cd1-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="e6cd1-106">**Odpowiedź:** Wybierz opcję **Dostarczanie dynamiczne.**</span><span class="sxs-lookup"><span data-stu-id="e6cd1-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="e6cd1-107">Aby uzyskać więcej informacji, zobacz [Dynamiczne dostarczanie w zasadach bezpiecznych załączników.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="e6cd1-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="e6cd1-108">**Przekieruj** sekcję załączników: Wybierz opcję Włącz przekierowywanie **,** a następnie wprowadź adres e-mail administratora globalnego platformy Microsoft 365, administratora zabezpieczeń lub analityka zabezpieczeń, który będzie badać złośliwe załączniki.</span><span class="sxs-lookup"><span data-stu-id="e6cd1-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="e6cd1-109">**Sekcja Zastosowano** do: Wybierz **pozycję Domena adresata to**, a następnie wybierz domenę.</span><span class="sxs-lookup"><span data-stu-id="e6cd1-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="e6cd1-110">Wybierz **pozycję dodaj**, a następnie wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="e6cd1-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="e6cd1-111">Po zakończeniu wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="e6cd1-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="e6cd1-112">Aby dowiedzieć się więcej, zobacz [Bezpieczne załączniki w programie Microsoft Defender dla usługi Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="e6cd1-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
