---
title: Antyspam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676507"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="2ef64-102">Rozwiązywanie problemów z dostarczaniem wiadomości e-mail dla kodu błędu 5.7.23</span><span class="sxs-lookup"><span data-stu-id="2ef64-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="2ef64-103">Sprawdź rekord DNS SPF dla domeny w publicznie dostępnym kontrolerze SPF lub DNS w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="2ef64-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="2ef64-104">Sprawdź, czy wiadomość wychodząca nie została zidentyfikowana jako spam przez firmę Microsoft i przekierowana przez [pulę dostarczania wysokiego ryzyka.](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="2ef64-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="2ef64-105">Wiadomości w puli dostarczania wysokiego ryzyka nie będą przechodzić kontroli SPF i dlatego nie będą akceptowane przez docelową organizację poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="2ef64-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="2ef64-106">Jeśli problem będzie się powtarzał, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="2ef64-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="2ef64-107">Zanotuj szczegółowy błąd zewnętrzny dostępny w komunikacie o odrzuceniu.</span><span class="sxs-lookup"><span data-stu-id="2ef64-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="2ef64-108">Pomoc techniczna firmy Microsoft może nie być w stanie pomóc dalej.</span><span class="sxs-lookup"><span data-stu-id="2ef64-108">Microsoft support may not be able to assist further.</span></span>
