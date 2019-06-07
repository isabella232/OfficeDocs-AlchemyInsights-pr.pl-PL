---
title: Ograniczanie Online programu SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761268"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="4b922-102">Ograniczanie Online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="4b922-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="4b922-103">Użytkownicy mogą otrzymywać 503 Serwer jest zajęty, błąd podczas próby przejdź do witryny programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4b922-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="4b922-104">Ten błąd może być spowodowany przez ograniczanie w ramach usługi programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b922-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4b922-105">SharePoint Online używa ograniczania do utrzymania optymalnej wydajności i niezawodności usług Online programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b922-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4b922-106">Limitów przepustowości liczba akcji użytkownika lub równoczesnych połączeń (przez skrypt lub kod) do zapobiec nadużywaniu zasobów.</span><span class="sxs-lookup"><span data-stu-id="4b922-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="4b922-107">Jeśli zostanie ograniczona, 99% czasu, to z powodu kodu niestandardowego.</span><span class="sxs-lookup"><span data-stu-id="4b922-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="4b922-108">Aby uzyskać więcej informacji na ograniczanie [należy unikać pobierania ograniczona lub zablokowany w dokumentacji Online programu SharePoint](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online), zobacz.</span><span class="sxs-lookup"><span data-stu-id="4b922-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="4b922-109">Jeśli uważasz, że ten błąd nie ma wpływu na ograniczanie, można sprawdzić, czy jest aktywne konserwacji występujące w dzierżawie przechodząc do [Centrum wiadomości](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="4b922-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="4b922-110">Wreszcie upewnij się, że odwiedź stronę [Usług zdrowotnych](https://portal.office.com/adminportal/home#/servicehealth) , aby sprawdzić, czy wszystkie klasyfikatory/incydentów, które może mieć miejsce.</span><span class="sxs-lookup"><span data-stu-id="4b922-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

