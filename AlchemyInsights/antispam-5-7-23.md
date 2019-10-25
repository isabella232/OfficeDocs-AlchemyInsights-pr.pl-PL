---
title: AntiSpam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682236"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="8e3a3-102">Napraw problemy z dostarczaniem wiadomości e-mail dla kodu błędu 5.7.23</span><span class="sxs-lookup"><span data-stu-id="8e3a3-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="8e3a3-103">Zweryfikuj rekord SPF DNS dla swojej domeny w publicznie dostępnym kontrolerze rekordów SPF lub DNS w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="8e3a3-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="8e3a3-104">Sprawdź, czy wiadomość wychodząca nie została zidentyfikowana jako spam przez pakiet Office 365 i kierowane przez [pulę dostawy wysokiego ryzyka](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="8e3a3-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="8e3a3-105">Wiadomości w puli dostaw wysokiego ryzyka nie przejdzie kontroli SPF i dlatego nie będą akceptowane przez organizację docelową pocztę e-mail.</span><span class="sxs-lookup"><span data-stu-id="8e3a3-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="8e3a3-106">Jeśli problem będzie się powtarzał, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail.</span><span class="sxs-lookup"><span data-stu-id="8e3a3-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="8e3a3-107">Zanotuj szczegółowy błąd zewnętrzny dostępny w wiadomości odbijanie.</span><span class="sxs-lookup"><span data-stu-id="8e3a3-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="8e3a3-108">Pomoc techniczna pakietu Office 365 może nie być w stanie udzielić dalszej pomocy.</span><span class="sxs-lookup"><span data-stu-id="8e3a3-108">Office 365 support may not be able to assist further.</span></span>