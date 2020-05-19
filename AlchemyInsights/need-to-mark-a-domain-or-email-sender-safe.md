---
title: Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281181"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="c30f4-102">Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?</span><span class="sxs-lookup"><span data-stu-id="c30f4-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="c30f4-103">Korzystanie z **list bezpiecznych nadawców nie jest zalecane,** ponieważ otwiera organizację na ataki spamowe, phish i spoofing.</span><span class="sxs-lookup"><span data-stu-id="c30f4-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="c30f4-104">Jeśli jednak istnieje wymóg biznesowy, **zalecamy** użycie w tym celu **[reguł przepływu poczty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="c30f4-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="c30f4-105">Nasze wskazówki zapewniają uwierzytelnianie nadawcy (weryfikuje, że domena wysyłająca nie jest sfałszowana).</span><span class="sxs-lookup"><span data-stu-id="c30f4-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="c30f4-106">**Uwaga:** Nie zalecamy zarządzania fałszywymi alarmami przy użyciu list bezpiecznych nadawców, ponieważ wyjątki od filtrowania spamu mogą otworzyć twoją organizację na ataki zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="c30f4-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="c30f4-107">Jeśli użytkownicy odbierają wiadomości niepoprawnie oznaczone jako spam lub wiadomości-śmieci, **[zgłoś wiadomości i pliki firmie Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="c30f4-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="c30f4-108">Należy unikać bezpiecznych nadawców w programie Outlook, listy dozwolonych nadawców lub listy dozwolonych domen w zasadach **antyspamowych,** ponieważ nadawcy omijają wszelką ochronę przed spamem, fałszem i phish oraz uwierzytelnianie nadawców (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="c30f4-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="c30f4-109">Ta metoda jest najlepiej używana tylko do testowania tymczasowego.</span><span class="sxs-lookup"><span data-stu-id="c30f4-109">This method is best used for temporary testing only.</span></span>
