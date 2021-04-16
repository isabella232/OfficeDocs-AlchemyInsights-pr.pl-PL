---
title: Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792142"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="d3fdb-102">Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?</span><span class="sxs-lookup"><span data-stu-id="d3fdb-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="d3fdb-103">Korzystanie z **list bezpiecznych nadawców** nie jest zalecane, ponieważ otwiera organizację na spam, wyłudzy i spoofing.</span><span class="sxs-lookup"><span data-stu-id="d3fdb-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="d3fdb-104">Jeśli jednak istnieją wymagania biznesowe, zalecamy używanie **w tym** celu reguł **[przepływu](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** poczty.</span><span class="sxs-lookup"><span data-stu-id="d3fdb-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="d3fdb-105">Nasze wskazówki zapewniają, że uwierzytelnianie nadawcy (sprawdza, czy wysyłanie domeny nie jest sfałszowane).</span><span class="sxs-lookup"><span data-stu-id="d3fdb-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="d3fdb-106">**Uwaga:** Nie zalecamy zarządzania wyników fałszywie dodatnich za pomocą list bezpiecznych nadawców, ponieważ wyjątki od filtrowania spamu mogą otworzyć Twoją organizację na ataki zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="d3fdb-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="d3fdb-107">Jeśli Twoi użytkownik otrzymuje wiadomości nieprawidłowo oznaczone jako spam lub wiadomości-śmieci, zgłoś te wiadomości **[i pliki do firmy Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="d3fdb-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="d3fdb-108">Należy unikać stosowania zasad bezpiecznych nadawców w programie  Outlook, listy dozwolonych nadawców lub listy domen dozwolonych w zasadach ochrony przed spamem, ponieważ nadawcy pomijają całą ochronę przed spamem, fałszem i wyłudzką oraz uwierzytelnianie nadawców (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="d3fdb-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="d3fdb-109">Ta metoda jest najlepsza w przypadku tylko testów tymczasowych.</span><span class="sxs-lookup"><span data-stu-id="d3fdb-109">This method is best used for temporary testing only.</span></span>
