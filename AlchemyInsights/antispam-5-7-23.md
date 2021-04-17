---
title: Ochrona przed spłacami — 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821421"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="82afa-102">Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodem błędu 5.7.23</span><span class="sxs-lookup"><span data-stu-id="82afa-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="82afa-103">Zweryfikuj rekord DNS SPF dla swojej domeny w publicznie dostępnym kontrolerze rekordu SPF lub DNS w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="82afa-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="82afa-104">Sprawdź, czy wiadomość wychodząca nie została zidentyfikowany przez firmę Microsoft jako spam i przekierowyowana przez pulę dostarczania [wysokiego ryzyka.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="82afa-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="82afa-105">Wiadomości w puli dostarczania wysokiego ryzyka nie będą podlegały testom SPF, a zatem nie będą akceptowane przez docelową organizację poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="82afa-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="82afa-106">Jeśli problem będzie nadal występował, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="82afa-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="82afa-107">Zanotuj szczegółowy błąd zewnętrzny dostępny w wiadomości zwracaowej.</span><span class="sxs-lookup"><span data-stu-id="82afa-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="82afa-108">Pomoc techniczna firmy Microsoft może nie być w stanie dalej pomóc.</span><span class="sxs-lookup"><span data-stu-id="82afa-108">Microsoft support may not be able to assist further.</span></span>
