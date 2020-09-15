---
title: 1332 OWA — reguły skrzynki odbiorczej nie są wykonywane dla skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721601"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="864aa-102">Reguła skrzynki odbiorczej nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="864aa-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="864aa-103">Sprawdź poniższe ustawienia w aplikacji Outlook w sieci Web:</span><span class="sxs-lookup"><span data-stu-id="864aa-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="864aa-104">Wiadomość może zostać przekierowana, przekazana lub wysłana automatycznie na podstawie reguł skrzynki odbiorczej tylko raz.</span><span class="sxs-lookup"><span data-stu-id="864aa-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="864aa-105">Reguła przekierowania (Reguła skrzynki odbiorczej lub reguła przepływu poczty, nazywana również regułą transportu) może dodać maksymalnie dziesięć adresatów przekierowania do wiadomości.</span><span class="sxs-lookup"><span data-stu-id="864aa-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="864aa-106">Aby uzyskać więcej informacji, zobacz [limity reguł dziennika, transportu i skrzynki odbiorczej](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="864aa-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="864aa-107">Reguły skrzynki odbiorczej nie działają w przypadku alternatywnej skrzynki pocztowej dziennika.</span><span class="sxs-lookup"><span data-stu-id="864aa-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="864aa-108">Aby uzyskać więcej informacji na temat alternatywnej skrzynki pocztowej rejestrowania, zobacz [alternatywna Skrzynka pocztowa dziennika](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="864aa-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="864aa-109">Aby rozwiązać te problemy, zobacz artykuł [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="864aa-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="864aa-110">Jeśli poprzednie problemy nie zostaną zastosowane, uruchom raport diagnostyczny reguły skrzynki odbiorczej przed eskalacją problemu do pomocy technicznej firmy Microsoft:</span><span class="sxs-lookup"><span data-stu-id="864aa-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="864aa-111">Otwórz skrzynkę pocztową w aplikacji Outlook w sieci Web i kliknij pozycję</span><span class="sxs-lookup"><span data-stu-id="864aa-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="864aa-112">**Ustawienia**  >  **Wyświetlanie wszystkich ustawień**  >  programu Outlook **Poczta**  >  **Regułami**.</span><span class="sxs-lookup"><span data-stu-id="864aa-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="864aa-113">U dołu strony kliknij pozycję **Jeśli reguły nie działają, kliknij tutaj, aby wygenerować raport diagnostyczny**.</span><span class="sxs-lookup"><span data-stu-id="864aa-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
