---
title: Rozwiązywanie problemów z wydajnością usługi OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 5416da63851de8b0b45e1d5c0cef24b03db40e6e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054964"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="30d6c-102">Rozwiązywanie problemów z wydajnością usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="30d6c-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="30d6c-103">Jeśli występuje mniejsza niż oczekiwana synchronizacja lub podobne problemy z wydajnością w usłudze OneDrive:</span><span class="sxs-lookup"><span data-stu-id="30d6c-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="30d6c-104">Potwierdź, że nie istnieją żadne znane problemy przy użyciu [pulpitu nawigacyjnego kondycji usługi](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="30d6c-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="30d6c-105">[Włącz pliki na żądanie](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) , aby uzyskać dostęp do wszystkich plików w usłudze OneDrive bez konieczności pobierania ich wszystkich i korzystania z miejsca w pamięci urządzenia.</span><span class="sxs-lookup"><span data-stu-id="30d6c-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="30d6c-106">[Zapoznaj się z najlepszymi praktykami](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) dotyczącymi planowania i wydajności sieci.</span><span class="sxs-lookup"><span data-stu-id="30d6c-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="30d6c-107">[Zmaksymalizuj szybkość wysyłania i pobierania](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), zwłaszcza Jeśli synchronizujesz urządzenie po raz pierwszy.</span><span class="sxs-lookup"><span data-stu-id="30d6c-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="30d6c-108">Jeśli synchronizujesz bibliotekę z ponad 100 000 elementów, synchronizacja OneDrive może wydawać się zatrzymany przez długi czas, lub stan pokazuje przetwarzanie 0KB xMB.</span><span class="sxs-lookup"><span data-stu-id="30d6c-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="30d6c-109">[Dowiedz się więcej o synchronizowaniu ponad 100 000 plików](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , a także o [obsługiwanym limitem plików 300 000 w usłudze OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="30d6c-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="30d6c-110">Gdy użytkownik przekroczy limity użycia, SharePoint Online ogranicza wszelkie dalsze żądania z tego konta użytkownika na krótki okres.</span><span class="sxs-lookup"><span data-stu-id="30d6c-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="30d6c-111">Wszystkie akcje użytkownika są ograniczane, gdy przepustnica jest w mocy.</span><span class="sxs-lookup"><span data-stu-id="30d6c-111">All user actions are throttled while the throttle is in effect.</span></span>
