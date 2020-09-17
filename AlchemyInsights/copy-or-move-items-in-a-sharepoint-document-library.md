---
title: Kopiowanie lub przenoszenie elementów w bibliotece dokumentów programu SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807129"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="c9159-102">Kopiowanie lub przenoszenie elementów w bibliotece dokumentów programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="c9159-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="c9159-103">Możesz kopiować i przenosić pliki, foldery i linki do różnych lokalizacji w bibliotece dokumentów.</span><span class="sxs-lookup"><span data-stu-id="c9159-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="c9159-104">Możesz również kopiować elementy między witrynami.</span><span class="sxs-lookup"><span data-stu-id="c9159-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="c9159-105">W przeglądarce przejdź do plików, folderów lub łączy, które chcesz przenieść, a następnie kliknij pozycję **Kopiuj do** lub **Przenieś do**.</span><span class="sxs-lookup"><span data-stu-id="c9159-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9159-106">Polecenia **Kopiuj** i **Przenieś do** nie są dostępne, jeśli korzystasz z klasycznego środowiska usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c9159-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="c9159-107">W obszarze **Wybierz miejsce docelowe**wybierz lokalizację, do której chcesz skopiować lub przenieść elementy, lub kliknij pozycję **Przeglądaj witryny** , aby wyświetlić pełną listę witryn.</span><span class="sxs-lookup"><span data-stu-id="c9159-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9159-108">Jeśli nie widzisz innych witryn wymienionych podczas kopiowania elementów, kopiowanie między witrynami nie zostało skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="c9159-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="c9159-109">Aby ją włączyć, przejdź do strony ustawień w centrum administracyjnym programu SharePoint i kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c9159-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="c9159-110">Aby utworzyć nowy folder, wybierz lokalizację w hierarchii folderów, kliknij pozycję **Nowy folder**, wprowadź nazwę folderu, a następnie kliknij znacznik wyboru, aby zapisać nazwę.</span><span class="sxs-lookup"><span data-stu-id="c9159-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="c9159-111">Kliknij pozycję **Kopiuj tutaj** lub **Przenieś tutaj**.</span><span class="sxs-lookup"><span data-stu-id="c9159-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9159-112">Możesz skopiować maksymalnie 500 MB plików i folderów jednocześnie.</span><span class="sxs-lookup"><span data-stu-id="c9159-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="c9159-113">> podczas kopiowania dokumentów z historią wersji zostanie skopiowana tylko Najnowsza wersja.</span><span class="sxs-lookup"><span data-stu-id="c9159-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="c9159-114">Podczas przenoszenia dokumentów ich historia jest również przenoszona.</span><span class="sxs-lookup"><span data-stu-id="c9159-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="c9159-115">Po przeniesieniu pliku będzie on nadal wyświetlany w katalogu źródłowym do momentu jego całkowitego przeniesienia do miejsca docelowego, a następnie zostanie usunięty.</span><span class="sxs-lookup"><span data-stu-id="c9159-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="c9159-116">Plik pozostanie w koszu witryny źródłowej po zakończeniu przenoszenia i będzie podlegać normalnemu harmonogramowi odtwarzania, chyba że użytkownik odzyskuje go z kosza.</span><span class="sxs-lookup"><span data-stu-id="c9159-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="c9159-117">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="c9159-117">For more information, see:</span></span>

 - <span data-ttu-id="c9159-118">[Przenoszenie lub kopiowanie plików w programie SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (artykuł pomocy technicznej pakietu Office)</span><span class="sxs-lookup"><span data-stu-id="c9159-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="c9159-119">[Przenoszenie plików z dowolnego folderu](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (artykuł w blogu społeczności Microsoft Technical Technical)</span><span class="sxs-lookup"><span data-stu-id="c9159-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  