---
title: Potrzebujesz pomocy w zakresie limitów wysyłania wiadomości e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357869"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6c7fb-102">Potrzebujesz pomocy w zakresie limitów wysyłania wiadomości e-mail?</span><span class="sxs-lookup"><span data-stu-id="6c7fb-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6c7fb-103">Poniżej znajduje się **limity wysyłania według projektu** wymuszane w usłudze.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6c7fb-104">Więcej informacji na temat tych limitów można znaleźć [tutaj](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="6c7fb-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6c7fb-105">Aby zniechęcić do dostarczania niechcianych wiadomości zbiorczych, stosujemy limity stawek dla odbiorców na użytkownika **do wszystkich wiadomości wychodzących i wewnętrznych.**</span><span class="sxs-lookup"><span data-stu-id="6c7fb-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6c7fb-106">We wszystkich jednostkach SKU limit ten wynosi **10 000 odbiorców dziennie.**</span><span class="sxs-lookup"><span data-stu-id="6c7fb-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6c7fb-107">Klienci, którzy muszą wysyłać legalną zbiorczą komercyjną wiadomość e-mail (na przykład biuletyny klientów) powinni korzystać z usług zewnętrznych dostawców, którzy specjalizują się w tych usługach.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6c7fb-108">**Uwaga:** Po osiągnięciu limitu szybkości adresatów wiadomości nie można wysyłać ze skrzynki pocztowej, dopóki liczba adresatów, którzy wysłali wiadomości w ciągu ostatnich 24 godzin, nie spadnie poniżej limitu.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6c7fb-109">Użytkownik nie będzie mógł wysyłać wiadomości do tego momentu.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6c7fb-110">Limit szybkości komunikatów **30 wiadomości na minutę** jest stosowany we wszystkich jednostkach SKU.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6c7fb-111">Określa, ile wiadomości użytkownik może wysyłać ze swojego konta usługi Exchange Online w określonym czasie.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6c7fb-112">**Maksymalna liczba adresatów dozwolonych w polach Do, DW i UDW** dla pojedynczej wiadomości e-mail we wszystkich jednostkach SKU wynosi **1000 adresatów.**</span><span class="sxs-lookup"><span data-stu-id="6c7fb-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6c7fb-113">Aby dostosować ten limit, przejdź [tutaj](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="6c7fb-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
