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
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733208"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="8b8eb-102">Rozwiązywanie problemów z wydajnością usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="8b8eb-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="8b8eb-103">Jeśli występują wolniejsze niż oczekiwano synchronizacji lub podobne problemy z wydajnością z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8b8eb-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="8b8eb-104">Upewnij się, że nie są znane żadne problemy przy użyciu [pulpitu nawigacyjnego kondycji usługi](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8b8eb-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="8b8eb-105">[Włącz pliki na żądanie,](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) aby uzyskać dostęp do wszystkich plików w usłudze OneDrive bez konieczności pobierania wszystkich z nich i używania miejsca na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="8b8eb-106">[Zapoznaj się z najlepszymi rozwiązaniami w](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) zakresie planowania i wydajności sieci.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="8b8eb-107">[Zmaksymalizuj szybkość przesyłania i pobierania](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), zwłaszcza jeśli synchronizujesz urządzenie po raz pierwszy.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="8b8eb-108">Jeśli synchronizujesz bibliotekę z więcej niż 100 000 elementów, synchronizacja usługi OneDrive może wydawać się zablokowana przez długi czas lub stan pokazuje przetwarzanie 0KB xMB."</span><span class="sxs-lookup"><span data-stu-id="8b8eb-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="8b8eb-109">[Dowiedz się więcej o synchronizowaniu ponad 100 000 plików,](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) a także [o obsługiwanym limicie 300 000 plików w usłudze OneDrive.](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="8b8eb-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="8b8eb-110">Gdy użytkownik przekroczy limity użycia, sharepoint online ogranicza wszelkie dalsze żądania z tego konta użytkownika na krótki okres.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="8b8eb-111">Wszystkie akcje użytkownika są ograniczane, gdy przepustnica jest w życie.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-111">All user actions are throttled while the throttle is in effect.</span></span>
