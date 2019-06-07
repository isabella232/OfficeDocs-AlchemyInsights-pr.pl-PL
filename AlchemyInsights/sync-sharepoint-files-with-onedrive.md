---
title: Synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757829"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="d0ee7-102">Synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji OneDrive</span><span class="sxs-lookup"><span data-stu-id="d0ee7-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="d0ee7-103">Polecenie Otwórz w Eksploratorze otwiera lokalne wystąpienia Eksploratora Windows, które wyświetli strukturę folderów na serwerze hostującym witrynę programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="d0ee7-104">W tym przypadku zalecamy [synchronizację plików programu SharePoint za pomocą nowego klienta synchronizacji OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> zawierającego funkcję [Pliki na żądanie](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), ponieważ zapewnia on lokalny dostęp do plików i oferuje najlepszą wydajność.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="d0ee7-105">W przypadku korzystania z opcji widoku Eksploratora zamiast z nowego klienta synchronizacji upewnij się, że postępujesz zgodnie z krokami i najważniejszymi wskazówkami przedstawionymi w poniższych artykułach.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="d0ee7-106">Rozwiązywanie problemów w usłudze SharePoint Online za pomocą polecenia „Otwórz w Eksploratorze”</span><span class="sxs-lookup"><span data-stu-id="d0ee7-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="d0ee7-107">Kopiowanie i przenoszenie plików biblioteki za pomocą polecenia Otwórz w Eksploratorze</span><span class="sxs-lookup"><span data-stu-id="d0ee7-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="d0ee7-108">Uwaga: przycisk Otwórz w Eksploratorze nie jest wyświetlany w nowym środowisku biblioteki.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="d0ee7-109">Kliknij listę rozwijaną Widok w prawym górnym rogu (nazwa listy rozwijanej zmienia się w zależności od bieżącego widoku), a następnie kliknij pozycję Wyświetl w Eksploratorze plików.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="d0ee7-110">W programie SharePoint do polecenia Otwórz w Eksploratorze używane są kontrolki ActiveX, więc jest ono obsługiwane tylko w programie Internet Explorer 10 lub 11.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="d0ee7-111">Polecenie Otwórz w Eksploratorze nie działa w systemie Windows przy użyciu przeglądarki Microsoft Edge, Google Chrome i Mozilla Firefox lub na platformie Mac.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="d0ee7-112">Z tego powodu opcja Widoku Eksploratora może być wyszarzona.</span><span class="sxs-lookup"><span data-stu-id="d0ee7-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="d0ee7-113">[Dlaczego przyciski na wstążce programu SharePoint są niedostępne lub wyszarzone](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="d0ee7-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

