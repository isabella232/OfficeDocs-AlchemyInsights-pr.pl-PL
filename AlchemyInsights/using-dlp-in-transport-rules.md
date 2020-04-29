---
title: Korzystanie z zasad DLP w regułach transportu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915189"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="6f475-102">Korzystanie z zasad DLP w regułach transportu</span><span class="sxs-lookup"><span data-stu-id="6f475-102">Using DLP in transport rules</span></span>

<span data-ttu-id="6f475-103">Aby zintegrować ochronę przed utratą danych (DLP) z istniejącym transportem, użyj warunku „**Jeśli wiadomość zawiera... Informacje poufne**” w ustawieniu Reguła transportu.</span><span class="sxs-lookup"><span data-stu-id="6f475-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="6f475-104">**Aby uzyskać więcej informacji, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="6f475-104">**For more details, see:**</span></span>

- <span data-ttu-id="6f475-105">Zintegrowane typy informacji poufnych zasad DLP w regułach transportu: [Integrowanie reguł informacji poufnych](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="6f475-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="6f475-106">Regułę można też testować przy użyciu testu zasad lub bez niego, korzystając z trybu testu w regule.</span><span class="sxs-lookup"><span data-stu-id="6f475-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="6f475-107">Przed rozpoczęciem testowania reguły należy odczekać 30 minut po jej utworzeniu.</span><span class="sxs-lookup"><span data-stu-id="6f475-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="6f475-108">Zobacz [Testowanie przepływu poczty e-mail/reguł transportu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="6f475-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="6f475-109">**Uwaga**: jeśli próbujesz zaimplementować nowe zasady DLP z regułami transportu w centrum administracyjnym programu Exchange, użyj [zasad DLP w Centrum zabezpieczeń i zgodności](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6f475-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
