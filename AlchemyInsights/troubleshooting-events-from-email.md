---
title: Rozwiązywanie problemów z pocztą E-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658744"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="9a9f3-102">Rozwiązywanie problemów z pocztą E-mail</span><span class="sxs-lookup"><span data-stu-id="9a9f3-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="9a9f3-103">Sprawdzanie, czy funkcja jest włączona dla skrzynki pocztowej: **Get-EventsFromEmailConfiguration <mailbox> -Identity**</span><span class="sxs-lookup"><span data-stu-id="9a9f3-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="9a9f3-104">Następnie sprawdź dzienniki "zdarzenia z poczty E-mail" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="9a9f3-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="9a9f3-105">W dziennikach "zdarzenia z poczty E-mail" Znajdź InternetMessageId pasujący do elementu w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="9a9f3-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="9a9f3-106">TrustScore określa, czy dany element został dodany, czy nie.</span><span class="sxs-lookup"><span data-stu-id="9a9f3-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="9a9f3-107">Zdarzenia zostaną dodane tylko wtedy, gdy TrustScore = "zaufane".</span><span class="sxs-lookup"><span data-stu-id="9a9f3-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="9a9f3-108">TrustScore jest określany na podstawie właściwości SPF, DKIM lub DMARC, które znajdują się w nagłówku wiadomości.</span><span class="sxs-lookup"><span data-stu-id="9a9f3-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="9a9f3-109">Aby wyświetlić te właściwości:</span><span class="sxs-lookup"><span data-stu-id="9a9f3-109">To view these properties:</span></span>

<span data-ttu-id="9a9f3-110">**Program Outlook dla komputerów stacjonarnych**</span><span class="sxs-lookup"><span data-stu-id="9a9f3-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="9a9f3-111">Otwórz element</span><span class="sxs-lookup"><span data-stu-id="9a9f3-111">Open the item</span></span>
- <span data-ttu-id="9a9f3-112">Plik — właściwości >-> nagłówki internetowe</span><span class="sxs-lookup"><span data-stu-id="9a9f3-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="9a9f3-113">lub</span><span class="sxs-lookup"><span data-stu-id="9a9f3-113">or</span></span>

<span data-ttu-id="9a9f3-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="9a9f3-114">**MFCMapi**</span></span>

- <span data-ttu-id="9a9f3-115">Przechodzenie do elementu w skrzynce odbiorczej</span><span class="sxs-lookup"><span data-stu-id="9a9f3-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="9a9f3-116">Szukaj PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="9a9f3-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="9a9f3-117">Te właściwości są określane i rejestrowane podczas transportu i routingu.</span><span class="sxs-lookup"><span data-stu-id="9a9f3-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="9a9f3-118">Aby uzyskać dalsze Rozwiązywanie problemów, może być konieczne wykonanie dodatkowych czynności w zakresie pomocy technicznej transportowej dotyczących błędów w programie SPF, DKIM i. lub DMARC.</span><span class="sxs-lookup"><span data-stu-id="9a9f3-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>