---
title: Ograniczanie przepustowości online programu SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751898"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="76f3b-102">Ograniczanie przepustowości online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="76f3b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="76f3b-103">Użytkownicy mogą otrzymać 503 serwer jest zajęty błąd podczas próby przejdź do witryny programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="76f3b-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="76f3b-104">Ten błąd może być spowodowany przez ograniczanie przepustowości w ramach usługi programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="76f3b-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="76f3b-105">Usługa SharePoint Online używa ograniczania przepustowości, aby zachować optymalną wydajność i niezawodność usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="76f3b-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="76f3b-106">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (przez skrypt lub kod), aby zapobiec nadmiernym użyciu zasobów.</span><span class="sxs-lookup"><span data-stu-id="76f3b-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="76f3b-107">Jeśli zostanie ograniczona, 99% czasu jest z powodu kodu niestandardowego.</span><span class="sxs-lookup"><span data-stu-id="76f3b-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="76f3b-108">Aby uzyskać więcej informacji na temat ograniczania przepustowości Zobacz, [Unikaj uzyskiwania ograniczane lub zablokowane w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="76f3b-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="76f3b-109">Jeśli uważasz, że ten błąd nie ma związku z ograniczania przepustowości, można sprawdzić, czy istnieje aktywnej konserwacji występujących w dzierżawie, przechodząc do [centrum wiadomości](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="76f3b-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="76f3b-110">Na koniec upewnij się, odwiedź stronę [kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth) , aby sprawdzić, czy wszystkie ostrzeżenia/incydentów, które mogą być występujące.</span><span class="sxs-lookup"><span data-stu-id="76f3b-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

