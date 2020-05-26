---
title: Blokuj pobieranie na łączach udostępniania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358036"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="f8a50-102">Blokuj pobieranie na łączach udostępniania</span><span class="sxs-lookup"><span data-stu-id="f8a50-102">Block download on sharing links</span></span>

<span data-ttu-id="f8a50-103">**Opcja Blokuj pobieranie** jest dostępna dla łączy tylko do **wyświetlania** dokumentów pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="f8a50-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="f8a50-104">Po wybraniu tej opcji osoby uzyskujące dostęp do pliku za pośrednictwem utworzonego łącza nie będą widzieć opcji pobierania, drukowania ani kopiowania pliku.</span><span class="sxs-lookup"><span data-stu-id="f8a50-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="f8a50-105">Administratorzy mogą kontrolować, czy ustawienie "pobieranie blokowe" jest wyświetlane tylko dla plików pakietu Office, czy nie, zmieniając `BlockDownloadLinksFileType` to ustawienie w poleceniach cmdlet [programu PowerShell set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) lub [Set-SPOSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="f8a50-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
