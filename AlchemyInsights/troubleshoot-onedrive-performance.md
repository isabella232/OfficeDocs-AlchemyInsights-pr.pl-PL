---
title: Rozwiązywanie problemów z wydajnością usługi OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757895"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="2de0f-102">Rozwiązywanie problemów z wydajnością usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="2de0f-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="2de0f-103">Jeśli wystąpił problem z synchronizacją mniejszą niż oczekiwana lub podobne problemy z wydajnością w usłudze OneDrive:</span><span class="sxs-lookup"><span data-stu-id="2de0f-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="2de0f-104">Upewnij się, że nie ma żadnych znanych problemów dotyczących korzystania z [pulpitu nawigacyjnego kondycja usługi](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2de0f-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="2de0f-105">[Włącz funkcję plików na żądanie](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , aby móc uzyskiwać dostęp do wszystkich plików w usłudze OneDrive bez konieczności pobierania ich wszystkich i używania miejsca do magazynowania na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="2de0f-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="2de0f-106">Zapoznaj się z [najważniejszymi wskazówkami](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) dotyczącymi planowania i wydajności sieci.</span><span class="sxs-lookup"><span data-stu-id="2de0f-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="2de0f-107">[Maksymalizuj szybkość przekazywania i pobierania](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), szczególnie jeśli synchronizacja urządzenia jest przeprowadzana po raz pierwszy.</span><span class="sxs-lookup"><span data-stu-id="2de0f-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="2de0f-108">Jeśli synchronizacja biblioteki obejmuje więcej niż 100 000 elementów, synchronizacja z usługą OneDrive może pozornie być zablokowana przez dłuższy czas lub stan wskazuje, że 0KB xMB.</span><span class="sxs-lookup"><span data-stu-id="2de0f-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="2de0f-109">[Dowiedz się więcej na temat synchronizowania więcej niż 100 000 plików](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , a także [limitu obsługi plików w usłudze OneDrive o wartości 300 000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="2de0f-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="2de0f-110">Gdy użytkownik przekroczy limity użycia, usługi SharePoint Online ograniczają wszelkie kolejne żądania od tego konta użytkownika przez krótki okres.</span><span class="sxs-lookup"><span data-stu-id="2de0f-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="2de0f-111">Wszystkie działania użytkowników są ograniczane, gdy obowiązuje przepustnica.</span><span class="sxs-lookup"><span data-stu-id="2de0f-111">All user actions are throttled while the throttle is in effect.</span></span>
