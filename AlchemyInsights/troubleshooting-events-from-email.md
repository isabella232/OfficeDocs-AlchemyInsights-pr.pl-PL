---
title: Rozwiązywanie problemów ze zdarzeniami z poczty e-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834849"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="90ed5-102">Rozwiązywanie problemów ze zdarzeniami z poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="90ed5-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="90ed5-103">Sprawdzanie, czy funkcja jest włączona dla skrzynki pocztowej: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="90ed5-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="90ed5-104">Następnie przyjrzyj się dziennikom "Zdarzenia z poczty **e-mail" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="90ed5-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="90ed5-105">W dziennikach "Events from Email" (Zdarzenia z poczty e-mail) znajdź element InternetMessageId, który odpowiada elementowi w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="90ed5-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="90ed5-106">Wartość TrustScore określa, czy element został dodany.</span><span class="sxs-lookup"><span data-stu-id="90ed5-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="90ed5-107">Zdarzenia zostaną dodane tylko wtedy, gdy trustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="90ed5-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="90ed5-108">Wartość TrustScore jest określana przez właściwości SPF, Dkim lub Dmarc, które znajdują się w nagłówku wiadomości.</span><span class="sxs-lookup"><span data-stu-id="90ed5-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="90ed5-109">Aby wyświetlić te właściwości:</span><span class="sxs-lookup"><span data-stu-id="90ed5-109">To view these properties:</span></span>

<span data-ttu-id="90ed5-110">**Klasyczny program Outlook**</span><span class="sxs-lookup"><span data-stu-id="90ed5-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="90ed5-111">Otwieranie elementu</span><span class="sxs-lookup"><span data-stu-id="90ed5-111">Open the item</span></span>
- <span data-ttu-id="90ed5-112">Plik — > właściwości -> nagłówków internetowych</span><span class="sxs-lookup"><span data-stu-id="90ed5-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="90ed5-113">lub</span><span class="sxs-lookup"><span data-stu-id="90ed5-113">or</span></span>

<span data-ttu-id="90ed5-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="90ed5-114">**MFCMapi**</span></span>

- <span data-ttu-id="90ed5-115">Przechodzenie do elementu w skrzynce odbiorczej</span><span class="sxs-lookup"><span data-stu-id="90ed5-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="90ed5-116">Poszukaj PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="90ed5-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="90ed5-117">Te właściwości są określane i rejestrowane podczas transportu i routingu.</span><span class="sxs-lookup"><span data-stu-id="90ed5-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="90ed5-118">W celu dalszego rozwiązywania problemów może być konieczne swoicie się z pomocą techniczną transportu w przypadku błędów SPF, DKIM i DMARC.</span><span class="sxs-lookup"><span data-stu-id="90ed5-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>