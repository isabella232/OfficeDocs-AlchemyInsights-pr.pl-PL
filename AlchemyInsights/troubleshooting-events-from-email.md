---
title: Rozwiązywanie problemów ze zdarzeniami z poczty e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569408"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c5044-102">Rozwiązywanie problemów ze zdarzeniami z poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="c5044-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c5044-103">Sprawdź, czy funkcja jest włączona dla skrzynki pocztowej: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="c5044-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c5044-104">Następnie spójrz na "Zdarzenia z wiadomości e-mail" dzienniki **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="c5044-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c5044-105">W dziennikach "Zdarzenia z wiadomości e-mail" znajdź identyfikator InternetMessageId, który pasuje do elementu w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="c5044-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c5044-106">TrustScore określa, czy element jest dodawany, czy nie.</span><span class="sxs-lookup"><span data-stu-id="c5044-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c5044-107">Zdarzenia zostaną dodane tylko wtedy, gdy TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="c5044-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c5044-108">TrustScore jest określana przez SPF, Dkim lub Dmarc właściwości, które znajdują się w nagłówku wiadomości.</span><span class="sxs-lookup"><span data-stu-id="c5044-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c5044-109">Aby wyświetlić te właściwości:</span><span class="sxs-lookup"><span data-stu-id="c5044-109">To view these properties:</span></span>

<span data-ttu-id="c5044-110">**Program Outlook dla komputerów stacjonarnych**</span><span class="sxs-lookup"><span data-stu-id="c5044-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c5044-111">Otwieranie elementu</span><span class="sxs-lookup"><span data-stu-id="c5044-111">Open the item</span></span>
- <span data-ttu-id="c5044-112">Właściwości pliku -> -> nagłówki internetowe</span><span class="sxs-lookup"><span data-stu-id="c5044-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c5044-113">lub</span><span class="sxs-lookup"><span data-stu-id="c5044-113">or</span></span>

<span data-ttu-id="c5044-114">**Mfcmapi**</span><span class="sxs-lookup"><span data-stu-id="c5044-114">**MFCMapi**</span></span>

- <span data-ttu-id="c5044-115">Przejdź do elementu w skrzynce odbiorczej</span><span class="sxs-lookup"><span data-stu-id="c5044-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c5044-116">Poszukaj PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c5044-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c5044-117">Właściwości te są określane i rejestrowane podczas transportu i routingu.</span><span class="sxs-lookup"><span data-stu-id="c5044-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c5044-118">Aby uzyskać dalsze rozwiązywanie problemów, może być konieczne monitorowanie obsługi transportu dotyczące błędów w filtrze SPF, DKIM i.lub DMARC.</span><span class="sxs-lookup"><span data-stu-id="c5044-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>