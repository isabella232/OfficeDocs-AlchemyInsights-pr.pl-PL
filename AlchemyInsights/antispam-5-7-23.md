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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506453"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="c0488-102">Rozwiązywanie problemów z dostarczaniem wiadomości e-mail dla kodu błędu 5.7.23</span><span class="sxs-lookup"><span data-stu-id="c0488-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="c0488-103">Sprawdź rekord DNS SPF dla domeny w publicznie dostępnym kontrolerze SPF lub DNS w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="c0488-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="c0488-104">Sprawdź, czy wiadomość wychodząca nie została zidentyfikowana jako spam przez firmę Microsoft i przekierowana przez [pulę dostarczania wysokiego ryzyka.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="c0488-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="c0488-105">Wiadomości w puli dostarczania wysokiego ryzyka nie będą przechodzić kontroli SPF i dlatego nie będą akceptowane przez docelową organizację poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="c0488-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="c0488-106">Jeśli problem będzie się powtarzał, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="c0488-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="c0488-107">Zanotuj szczegółowy błąd zewnętrzny dostępny w komunikacie o odrzuceniu.</span><span class="sxs-lookup"><span data-stu-id="c0488-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="c0488-108">Pomoc techniczna firmy Microsoft może nie być w stanie pomóc dalej.</span><span class="sxs-lookup"><span data-stu-id="c0488-108">Microsoft support may not be able to assist further.</span></span>
