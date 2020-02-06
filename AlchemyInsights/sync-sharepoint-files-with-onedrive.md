---
title: Rozwiązywanie problemów w usłudze SharePoint Online za pomocą polecenia „Otwórz w Eksploratorze”
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 08/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 09d0d76f8c61f7fcd21a58527e220b65f123654d
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770289"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b7b5b-102">Rozwiązywanie problemów w usłudze SharePoint Online za pomocą polecenia „Otwórz w Eksploratorze”</span><span class="sxs-lookup"><span data-stu-id="b7b5b-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="b7b5b-103">Zalecamy [synchronizację plików programu SharePoint za pomocą nowego klienta synchronizacji OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) zawierającego funkcję [Pliki na żądanie](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), ponieważ zapewnia on lokalny dostęp do plików i oferuje najlepszą wydajność.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="b7b5b-104">W celu rozwiązania problemów z funkcją „Otwórz w Eksploratorze” wykonaj czynności opisane w poniższych artykułach:</span><span class="sxs-lookup"><span data-stu-id="b7b5b-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b7b5b-105">Rozwiązywanie problemów w usłudze SharePoint Online za pomocą polecenia „Otwórz w Eksploratorze”</span><span class="sxs-lookup"><span data-stu-id="b7b5b-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="b7b5b-106">Kopiowanie i przenoszenie plików biblioteki za pomocą polecenia Otwórz w Eksploratorze</span><span class="sxs-lookup"><span data-stu-id="b7b5b-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="b7b5b-107">**Uwaga:**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-107">**Note:**</span></span>
>
>- <span data-ttu-id="b7b5b-108">Przycisk Otwórz w Eksploratorze nie jest wyświetlany w nowym środowisku biblioteki.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-108">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b7b5b-109">Wybierz listę rozwijaną **Widok** w prawym górnym rogu (nazwa listy rozwijanej zmienia się w zależności od bieżącego widoku), a następnie wybierz pozycję **Wyświetl w Eksploratorze plików**.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
>- <span data-ttu-id="b7b5b-110">Polecenie Otwórz w Eksploratorze jest obsługiwane tylko w programie Internet Explorer 10 lub 11.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-110">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b7b5b-111">Polecenie Otwórz w Eksploratorze nie działa w systemie Windows przy użyciu przeglądarki Microsoft Edge, Google Chrome i Mozilla Firefox lub na platformie Mac.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b7b5b-112">Z tego powodu opcja Widoku Eksploratora może być wyszarzona.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-112">Due to this reason, the Explorer View option may be grayed out.</span></span>


