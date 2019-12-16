---
title: Ograniczanie przepustowości online programu SharePoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048626"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="7e6f9-102">Ograniczanie przepustowości online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e6f9-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="7e6f9-103">Użytkownicy mogą otrzymać 503 serwer jest zajęty błąd podczas próby przejdź do witryny programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="7e6f9-104">Ten błąd może być spowodowany przez ograniczanie przepustowości w ramach usługi programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7e6f9-105">Usługa SharePoint Online używa ograniczania przepustowości, aby zachować optymalną wydajność i niezawodność usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7e6f9-106">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (przez skrypt lub kod), aby zapobiec nadmiernym użyciu zasobów.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="7e6f9-107">Jeśli zostanie ograniczona, 99% czasu jest z powodu kodu niestandardowego.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="7e6f9-108">Aby uzyskać więcej informacji na temat ograniczania przepustowości Zobacz, [Unikaj uzyskiwania ograniczane lub zablokowane w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7e6f9-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="7e6f9-109">Jeśli uważasz, że ten błąd nie ma związku z ograniczania przepustowości, można sprawdzić, czy istnieje aktywnej konserwacji występujących w dzierżawie, przechodząc do [centrum wiadomości](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="7e6f9-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="7e6f9-110">Na koniec upewnij się, odwiedź stronę [kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth) , aby sprawdzić, czy wszystkie ostrzeżenia/incydentów, które mogą być występujące.</span><span class="sxs-lookup"><span data-stu-id="7e6f9-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

