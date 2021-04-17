---
title: Potrzebujesz pomocy w zakresie limitów wysyłania wiadomości e-mail?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836289"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="ce4fa-102">Potrzebujesz pomocy w zakresie limitów wysyłania wiadomości e-mail?</span><span class="sxs-lookup"><span data-stu-id="ce4fa-102">Need help with email sending limits?</span></span>

<span data-ttu-id="ce4fa-103">Poniżej znajdują się **zgodne z projektem limity wysyłania** egzekwowane w usłudze.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="ce4fa-104">Więcej informacji na temat tych ograniczeń znajduje się [tutaj](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="ce4fa-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="ce4fa-105">Aby zniechęcić do dostarczania niechcianych wiadomości masowych, stosujemy limity liczby **odbiorców na użytkownika do wszystkich wiadomości wychodzących i wewnętrznych**.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="ce4fa-106">We wszystkich jednostkach SKU ten limit wynosi **10 000 adresatów dziennie**.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="ce4fa-107">Klienci, którzy muszą wysyłać legalne, masowe wiadomości e-mail (na przykład biuletyny dla klientów), powinni korzystać z usług zewnętrznych dostawców specjalizujących się w tych usługach.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="ce4fa-108">**Uwaga**: po osiągnięciu limitu liczby adresatów nie można wysyłać wiadomości ze skrzynki pocztowej, dopóki liczba adresatów, do których wysłano wiadomości w ciągu ostatnich 24 godzin, nie spadnie poniżej limitu.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="ce4fa-109">Do tego momentu użytkownik nie będzie mógł wysyłać wiadomości.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="ce4fa-110">Limit szybkości przesyłania wiadomości wynoszący **30 wiadomości na minutę** jest stosowany we wszystkich jednostkach SKU.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="ce4fa-111">Określa, ile wiadomości użytkownik może wysłać ze swojego konta usługi Exchange Online w określonym czasie.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="ce4fa-112">**Maksymalna liczba adresatów dozwolona w polach Do, DW i UDW** dla pojedynczej wiadomości e-mail we wszystkich jednostkach SKU to **1000 adresatów**.</span><span class="sxs-lookup"><span data-stu-id="ce4fa-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="ce4fa-113">Aby dostosować ten limit, przejdź [tutaj](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="ce4fa-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
