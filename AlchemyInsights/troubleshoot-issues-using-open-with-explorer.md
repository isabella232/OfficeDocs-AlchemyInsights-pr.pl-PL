---
title: Rozwiązywanie problemów z pomocą Otwórz w Eksploratorze
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759304"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="9452c-102">Rozwiązywanie problemów z Otwórz w Eksploratorze</span><span class="sxs-lookup"><span data-stu-id="9452c-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="9452c-103">Rozwiązywanie typowych problemów z otwieraniem biblioteki dokumentów programu SharePoint lub za pomocą polecenia **Otwórz w Eksploratorze** OneDrive:</span><span class="sxs-lookup"><span data-stu-id="9452c-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="9452c-104">Użyj programu Internet Explorer 10 lub Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="9452c-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="9452c-105">**Otwórz w Eksploratorze** jest niezgodna z Edge firmy Microsoft, Google Chrome, Firefox i innych.</span><span class="sxs-lookup"><span data-stu-id="9452c-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9452c-106">**Otwórz w Eksploratorze** jest wyłączona we wszystkich przeglądarkach oprócz programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9452c-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="9452c-107">**Otwórz w Eksploratorze** jest niedostępna w nowoczesne doświadczenie dla bibliotek programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9452c-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="9452c-108">Użyj zamiast tego **widoku w Eksploratorze plik** .</span><span class="sxs-lookup"><span data-stu-id="9452c-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="9452c-109">Wybierz **Opcje widoku** \> **Widok w Eksploratorze plik**.</span><span class="sxs-lookup"><span data-stu-id="9452c-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="9452c-110">Widok w Eksploratorze plik jest niezgodny z Microsoft Edge, Google Chrome, Firefox i inne.</span><span class="sxs-lookup"><span data-stu-id="9452c-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9452c-111">**Wyświetlanie w Eksploratorze plików** w dostępne tylko w programie Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9452c-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="9452c-112">Upewnij się, że jest uruchomiona usługa WebClient.</span><span class="sxs-lookup"><span data-stu-id="9452c-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="9452c-113">W polu wyszukiwania systemu Windows, typ uruchomienia, wybierz aplikację pulpitu, uruchom, wpisz services.msc i naciśnij klawisz Enter.</span><span class="sxs-lookup"><span data-stu-id="9452c-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="9452c-114">Przewiń w dół do usługi WebClient i upewnij się, że w kolumnie **Stan** wyświetlana "Działa".</span><span class="sxs-lookup"><span data-stu-id="9452c-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="9452c-115">Jeśli tak nie jest, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij **OK**.</span><span class="sxs-lookup"><span data-stu-id="9452c-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9452c-116">(Być może trzeba najpierw włączyć usługę przez wybranie w polu **Typ uruchomienia** **Ręczny** lub **Automatyczny** ).</span><span class="sxs-lookup"><span data-stu-id="9452c-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9452c-117">Otwieranie biblioteki w Eksploratorze plik jest przydatny, jeśli trzeba kopiować lub przenosić wiele plików lub folderów po, ale jeśli chcesz regularnie pracują w bibliotece, firma Microsoft zaleca synchronizację.</span><span class="sxs-lookup"><span data-stu-id="9452c-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="9452c-118">Rozwiązywać problemy z otwieraniem w Eksploratorze plików, zobacz temat [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9452c-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9452c-119">Aby uzyskać informacje dotyczące konfigurowania synchronizacji zobacz [pliki synchronizacji programu SharePoint z nowego klienta synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9452c-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="9452c-120">Zobacz artykuł [sposób korzystania z polecenia "Otwórz z Eksploratora" rozwiązywania problemów w dokumentacji Online programu SharePoint](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="9452c-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

