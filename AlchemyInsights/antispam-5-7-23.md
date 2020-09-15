---
title: AntiSpam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717335"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="cc501-102">Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodem błędu 5.7.23</span><span class="sxs-lookup"><span data-stu-id="cc501-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="cc501-103">Sprawdź rekord SPF DNS dla swojej domeny w publicznie dostępnym narzędziu SPF lub Sprawdzanie rekordów DNS w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="cc501-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="cc501-104">Upewnij się, że wiadomość wychodząca nie została zidentyfikowana jako spam przez firmę Microsoft i przekierowana przez [pulę dostarczania wysokiego ryzyka](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="cc501-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="cc501-105">Wiadomości w puli dostarczania wysokiego ryzyka nie będą przekazywać testów SPF, więc nie zostaną zaakceptowane przez docelową organizację poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="cc501-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="cc501-106">Jeśli problem będzie nadal występował, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="cc501-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="cc501-107">Zanotuj szczegółowy błąd zewnętrzny, który jest dostępny w wiadomości odskakującej.</span><span class="sxs-lookup"><span data-stu-id="cc501-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="cc501-108">Pomoc techniczna firmy Microsoft może nie być w stanie pomóc dalej.</span><span class="sxs-lookup"><span data-stu-id="cc501-108">Microsoft support may not be able to assist further.</span></span>
