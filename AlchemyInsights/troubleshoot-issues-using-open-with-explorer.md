---
title: Rozwiązywanie problemów z użyciem funkcji Otwórz w Eksploratorze
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742743"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="dc6b1-102">Rozwiązywanie problemów z programem Otwórz w Eksploratorze</span><span class="sxs-lookup"><span data-stu-id="dc6b1-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="dc6b1-103">Rozwiązywanie typowych problemów z otwieraniem biblioteki dokumentów w programie SharePoint lub OneDrive za pomocą polecenia **Otwórz za pomocą Eksploratora** :</span><span class="sxs-lookup"><span data-stu-id="dc6b1-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="dc6b1-104">Użyj programu Internet Explorer 10 lub Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="dc6b1-105">**Otwórz w Eksploratorze** nie jest kompatybilny z Microsoft Edge, Google Chrome, Firefox i innych.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="dc6b1-106">**Otwórz za pomocą Eksploratora** jest wyłączony we wszystkich przeglądarkach z wyjątkiem programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="dc6b1-107">**Otwórz za pomocą Eksploratora** nie jest dostępna w nowoczesnych środowisko dla bibliotek programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="dc6b1-108">Zamiast tego użyj **widoku w Eksploratorze plików** .</span><span class="sxs-lookup"><span data-stu-id="dc6b1-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="dc6b1-109">Wybierz widok **opcji** \> widoku **w Eksploratorze plików**.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="dc6b1-110">Widok w Eksploratorze plików nie jest kompatybilny z Microsoft Edge, Google Chrome, Firefox i innych.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="dc6b1-111">**Widok w Eksploratorze plików** dostępny tylko w programie Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="dc6b1-112">Upewnij się, że usługa WebClient jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="dc6b1-113">W polu wyszukiwania systemu Windows wpisz Uruchom, wybierz Uruchom aplikację pulpitu, wpisz Services. msc, a następnie naciśnij Enter.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="dc6b1-114">Przewiń w dół do usługi WebClient i upewnij się, że w kolumnie **stan** jest wyświetlana "uruchomiona".</span><span class="sxs-lookup"><span data-stu-id="dc6b1-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="dc6b1-115">Jeśli nie, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="dc6b1-116">(Najpierw należy włączyć tę usługę, wybierając opcję **ręczny** lub **automatyczny** w polu **Typ uruchomienia** ).</span><span class="sxs-lookup"><span data-stu-id="dc6b1-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="dc6b1-117">Otwarcie biblioteki w Eksploratorze plików jest przydatne, jeśli trzeba skopiować lub przenieść wiele plików i folderów raz, ale jeśli chcesz regularnie pracować w bibliotece, zalecamy synchronizację.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="dc6b1-118">Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="dc6b1-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="dc6b1-119">Aby uzyskać informacje o konfigurowaniu synchronizacji, zobacz [synchronizowanie plików programu SharePoint z nowym klientem synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="dc6b1-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="dc6b1-120">Zapoznaj się z artykułem [jak używać polecenia "Otwórz w Eksploratorze" rozwiązywać problemy w programie SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) Aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="dc6b1-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

