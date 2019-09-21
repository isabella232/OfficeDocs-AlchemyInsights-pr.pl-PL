---
title: Wychodzące wiadomości e-mail do folderu wiadomości-śmieci
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062816"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="76987-102">Wychodzące wiadomości e-mail do folderu wiadomości-śmieci</span><span class="sxs-lookup"><span data-stu-id="76987-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="76987-103">Jeśli widzisz wiadomości wychodzące oznaczone jako wiadomości-śmieci, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="76987-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="76987-104">Jeśli jeszcze tego nie zrobiono, rozważ [skonfigurowanie powiadomień dotyczących spamu wychodzącego](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="76987-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="76987-105">Użyj [śledzenia wiadomości](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) , aby sprawdzić, czy wiadomość wychodząca ma wartość zdarzenia **spam** z dodatkowymi szczegółami: **Użyj puli dostaw wysokiego ryzyka**.</span><span class="sxs-lookup"><span data-stu-id="76987-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="76987-106">W przypadku tych wiadomości sprawdź zawartość wiadomości, aby zobaczyć, co może być traktowane jako spam.</span><span class="sxs-lookup"><span data-stu-id="76987-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="76987-107">Na przykład podpisy mogą czasami powodować problemy dla wielu użytkowników.</span><span class="sxs-lookup"><span data-stu-id="76987-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="76987-108">Jeśli masz wiele przykładów uzasadnionych wiadomości wychodzących, które są oznaczone jako wiadomości-śmieci, Otwórz bilet pomocy technicznej i poprosić agenta pomocy technicznej, aby przesłać wiadomości jako fałszywych alarmów do naszych analityków spamu.</span><span class="sxs-lookup"><span data-stu-id="76987-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="76987-109">Przygotuj się do dostarczania przykładowych wiadomości, które zawierają wszystkie nagłówki wiadomości.</span><span class="sxs-lookup"><span data-stu-id="76987-109">Be prepared to provide sample messages that include all message headers.</span></span>
