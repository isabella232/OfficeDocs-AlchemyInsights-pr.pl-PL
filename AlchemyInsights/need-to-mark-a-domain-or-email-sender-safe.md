---
title: Chcesz bezpiecznie oznaczyć domenę lub nadawcę wiadomości e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803255"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="605e2-102">Chcesz bezpiecznie oznaczyć domenę lub nadawcę wiadomości e-mail?</span><span class="sxs-lookup"><span data-stu-id="605e2-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="605e2-103">Korzystanie z **list bezpiecznych nadawców nie jest zalecane** , ponieważ powoduje otwarcie organizacji na ataki z spamem, phishingiem i fałszowaniem.</span><span class="sxs-lookup"><span data-stu-id="605e2-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="605e2-104">Jeśli jednak istnieje wymóg biznesowy, **zalecamy** korzystanie z **[reguł przepływu poczty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="605e2-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="605e2-105">Nasze wskazówki gwarantują uwierzytelnienie nadawcy (sprawdzanie, że domena wysłana nie jest fałszywa).</span><span class="sxs-lookup"><span data-stu-id="605e2-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="605e2-106">**Uwaga**: nie zalecamy zarządzania fałszywymi wynikami pozytywnymi przy użyciu list bezpiecznych nadawców, ponieważ wyjątki dotyczące filtrowania spamu mogą otwierać organizację w celu zapewnienia bezpieczeństwa.</span><span class="sxs-lookup"><span data-stu-id="605e2-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="605e2-107">Jeśli użytkownik otrzyma wiadomości niepoprawnie oznaczone jako spam lub wiadomości-śmieci, prosimy **[o zgłoszenie wiadomości i plików do firmy Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="605e2-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="605e2-108">**Można uniknąć** bezpiecznych nadawców w programie Outlook, listy dozwolonych nadawców lub listy dozwolonych domen w zasadach ochrony przed spamem, ponieważ nadawcy pomijają wszystkie spam, fałszowanie i ochronę przed wirusami oraz uwierzytelnianie nadawcy (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="605e2-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="605e2-109">Ta metoda jest najbardziej przydatna tylko w przypadku tymczasowych testów.</span><span class="sxs-lookup"><span data-stu-id="605e2-109">This method is best used for temporary testing only.</span></span>
