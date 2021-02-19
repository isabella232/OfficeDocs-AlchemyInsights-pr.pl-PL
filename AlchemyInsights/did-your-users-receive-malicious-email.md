---
title: Czy użytkownicy otrzymali złośliwą wiadomość e-mail?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291802"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="91c1f-102">Czy użytkownicy otrzymali złośliwą wiadomość e-mail?</span><span class="sxs-lookup"><span data-stu-id="91c1f-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="91c1f-103">Teraz możesz zgłosić złośliwą wiadomość e-mail do firmy Microsoft za pomocą opcji [Przesłane zgłoszenia przez administratorów w Centrum zabezpieczeń i zgodności](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="91c1f-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="91c1f-104">Wiadomości przesłane w obszarze [przesłane zgłoszenia przez administratorów](https://sip.protection.office.com/reportsubmission) są skanowane, a następujące wyniki są wyświetlane w menu wysuwanym **szczegółów**:</span><span class="sxs-lookup"><span data-stu-id="91c1f-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="91c1f-105">Jeśli wystąpił błąd w uwierzytelnianiu wiadomości e-mail nadawcy w czasie dostarczania.</span><span class="sxs-lookup"><span data-stu-id="91c1f-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="91c1f-106">Informacje na temat wskazówek dotyczących zasad, które mogły wpłynąć na werdykt wiadomości lub go pominąć.</span><span class="sxs-lookup"><span data-stu-id="91c1f-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="91c1f-107">Bieżące wyniki detonacji, aby sprawdzić, czy adresy URL lub pliki zawarte w wiadomości były złośliwe.</span><span class="sxs-lookup"><span data-stu-id="91c1f-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="91c1f-108">Informacja zwrotna od mechanizmów oceniających</span><span class="sxs-lookup"><span data-stu-id="91c1f-108">Feedback from graders</span></span>

<span data-ttu-id="91c1f-109">Jeśli wykryto pominięcie, ponowne skanowanie powinno zostać zakończone w ciągu kilku minut.</span><span class="sxs-lookup"><span data-stu-id="91c1f-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="91c1f-110">Jeśli w uwierzytelnianiu wiadomości e-mail nie wystąpił błąd, bądź pominięcie nie miało wpływu na dostarczenie, wtedy uzyskanie informacji zwrotnej od mechanizmów oceniających może zająć nawet jeden dzień.</span><span class="sxs-lookup"><span data-stu-id="91c1f-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="91c1f-111">Jeśli nie zgadzasz się z ostatecznym werdyktem dotyczącym wiadomości, adresu URL lub pliku (zablokowany lub niezablokowany), prześlij ponownie wiadomość po upływie jednego dnia w celu wykonania ponownego skanowania.</span><span class="sxs-lookup"><span data-stu-id="91c1f-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="91c1f-112">Istnieje wysokie prawdopodobieństwo, że werdykt może ulec zmianie po ponownym przesłaniu wiadomości.</span><span class="sxs-lookup"><span data-stu-id="91c1f-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="91c1f-113">W międzyczasie możesz usunąć złośliwą wiadomość e-mail ze skrzynek odbiorczych użytkowników, wykonując czynności opisane w [tym artykule](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="91c1f-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="91c1f-114">Klienci w ramach ochrony usługi Office 365 w usłudze Microsoft Defender mogą:</span><span class="sxs-lookup"><span data-stu-id="91c1f-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="91c1f-115">użyć [eksploratora zagrożeń w celu znalezienie i usunięcia podejrzanej wiadomości e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="91c1f-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="91c1f-116">[użyć bezpiecznych linków do zablokowania dostępu](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) do złośliwego adresu URL</span><span class="sxs-lookup"><span data-stu-id="91c1f-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="91c1f-117">śledzić użytkowników, którzy kliknęli i uzyskali dostęp do złośliwych adresów URL: [wyświetl adres URL wyłudzający informacje i kliknij dane dotyczące werdyktu](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="91c1f-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="91c1f-118">ręcznie[uruchomić zautomatyzowane badanie](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="91c1f-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="91c1f-119">Możesz też zabezpieczyć się przed złośliwymi plikami i adresami URL, wykonując czynności opisane w artykule [Ochrona przed złośliwymi adresami URL i plikami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="91c1f-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>