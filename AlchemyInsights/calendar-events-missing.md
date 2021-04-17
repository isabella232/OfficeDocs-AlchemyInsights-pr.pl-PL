---
title: Brakuje lub nie można zaktualizować zdarzeń kalendarza
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837385"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="22f91-102">Zdarzenia kalendarza nie są aktualizowane lub nie są aktualizowane</span><span class="sxs-lookup"><span data-stu-id="22f91-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="22f91-103">Jeśli brakuje elementów kalendarza lub nie jest aktualizowana, zacznij od pozycji liczba elementów we właściwościach folderu Kalendarz w programie Outlook:</span><span class="sxs-lookup"><span data-stu-id="22f91-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="22f91-104">Kliknij prawym przyciskiem myszy folder Kalendarz **użytkownika, którego dotyczy** problem, a następnie wybierz pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="22f91-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="22f91-105">Wybierz **kartę Synchronizacja.**</span><span class="sxs-lookup"><span data-stu-id="22f91-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="22f91-106">Jeśli liczba elementów nie jest taka sama między folderem Serwer a folderem trybu offline:</span><span class="sxs-lookup"><span data-stu-id="22f91-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="22f91-107">Wyróżnij  folder Kalendarz.</span><span class="sxs-lookup"><span data-stu-id="22f91-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="22f91-108">Przejdź do karty / **Wysyłanie/odbieranie,** a następnie wybierz pozycję **Aktualizuj folder**.</span><span class="sxs-lookup"><span data-stu-id="22f91-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="22f91-109">Jeśli twój kalendarz nadal się nie aktualizuje lub brakuje zdarzeń, pobierz narzędzie do sprawdzania kalendarzy dla programu Outlook z Centrum [pobierania Microsoft.](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="22f91-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="22f91-110">Określ, czy w folderze kalendarza znajduje się więcej niż 5000 elementów, ponieważ może to powodować symptomy, takie jak nie zaktualizowano spotkań kalendarza lub błędy spotkania.</span><span class="sxs-lookup"><span data-stu-id="22f91-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="22f91-111">Aby uzyskać więcej informacji, zobacz Problemy z wydajnością programu Outlook w przypadku zbyt wielu elementów lub folderów w trybie buforowanej wersji ost lub [pst.](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)</span><span class="sxs-lookup"><span data-stu-id="22f91-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>