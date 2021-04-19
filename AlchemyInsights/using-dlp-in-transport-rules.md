---
title: Korzystanie z zasad DLP w regułach transportu
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827226"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="c150d-102">Korzystanie z zasad DLP w regułach transportu</span><span class="sxs-lookup"><span data-stu-id="c150d-102">Using DLP in transport rules</span></span>

<span data-ttu-id="c150d-103">Aby zintegrować ochronę przed utratą danych (DLP) z istniejącym transportem, użyj warunku „**Jeśli wiadomość zawiera... Informacje poufne**” w ustawieniu Reguła transportu.</span><span class="sxs-lookup"><span data-stu-id="c150d-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="c150d-104">**Aby uzyskać więcej informacji, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="c150d-104">**For more details, see:**</span></span>

- <span data-ttu-id="c150d-105">Zintegrowane typy informacji poufnych zasad DLP w regułach transportu: [Integrowanie reguł informacji poufnych](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="c150d-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="c150d-106">Regułę można też testować przy użyciu testu zasad lub bez niego, korzystając z trybu testu w regule.</span><span class="sxs-lookup"><span data-stu-id="c150d-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="c150d-107">Przed rozpoczęciem testowania reguły należy odczekać 30 minut po jej utworzeniu.</span><span class="sxs-lookup"><span data-stu-id="c150d-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="c150d-108">Zobacz [Testowanie przepływu poczty e-mail/reguł transportu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="c150d-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="c150d-109">**Uwaga**: jeśli próbujesz zaimplementować nowe zasady DLP z regułami transportu w centrum administracyjnym programu Exchange, użyj [zasad DLP w Centrum zabezpieczeń i zgodności](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c150d-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
