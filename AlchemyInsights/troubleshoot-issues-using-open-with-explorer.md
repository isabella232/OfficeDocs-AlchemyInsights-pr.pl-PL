---
title: Rozwiązywanie problemów z używaniem funkcji Otwórz w Eksploratorze
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759702"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="9e0e8-102">Rozwiązywanie problemów z otwieraniem z Eksploratorem</span><span class="sxs-lookup"><span data-stu-id="9e0e8-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="9e0e8-103">Rozwiązywanie typowych problemów z otwieraniem biblioteki dokumentów w programie SharePoint lub OneDrive przy użyciu polecenia **Otwórz z Eksploratorem:**</span><span class="sxs-lookup"><span data-stu-id="9e0e8-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="9e0e8-104">Użyj programu Internet Explorer 10 lub Programu Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="9e0e8-105">**Otwórz z Explorer** nie jest kompatybilny z Microsoft Edge, Google Chrome, Firefox i innych.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9e0e8-106">**Otwórz za pomocą Eksploratora** jest wyłączona we wszystkich przeglądarkach z wyjątkiem programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="9e0e8-107">**Otwórz za pomocą Eksploratora** nie jest dostępna w nowoczesnym środowiskach dla bibliotek programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="9e0e8-108">Zamiast tego użyj **widoku w Eksploratorze** plików.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="9e0e8-109">Wybierz pozycję **Opcje** \> widoku **Widok w Eksploratorze plików**.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="9e0e8-110">Widok w Eksploratorze plików nie jest zgodny z przeglądarkami Microsoft Edge, Google Chrome, Firefox i innymi.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9e0e8-111">**Wyświetl w Eksploratorze plików** dostępny tylko w programie Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="9e0e8-112">Upewnij się, że usługa WebClient jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="9e0e8-113">W polu wyszukiwania systemu Windows wpisz polecenie Uruchom aplikację klasyczną, wpisz services.msc, a następnie naciśnij klawisz Enter.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="9e0e8-114">Przewiń w dół do usługi WebClient i upewnij się, że w kolumnie **Stan** jest wyświetlana "Uruchomiona".</span><span class="sxs-lookup"><span data-stu-id="9e0e8-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="9e0e8-115">Jeśli tak nie jest, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9e0e8-116">(Może być konieczne włączenie usługi, wybierając opcję **Ręczna** lub **Automatyczna** w polu **Typ uruchamiania).**</span><span class="sxs-lookup"><span data-stu-id="9e0e8-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9e0e8-117">Otwieranie biblioteki w Eksploratorze plików jest przydatne, jeśli chcesz raz skopiować lub przenieść wiele plików i folderów, ale jeśli chcesz regularnie pracować w bibliotece, zalecamy jej synchronizację.</span><span class="sxs-lookup"><span data-stu-id="9e0e8-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="9e0e8-118">Aby rozwiązać problemy z otwieraniem się w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9e0e8-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9e0e8-119">Aby uzyskać informacje dotyczące konfigurowania synchronizacji, zobacz [Synchronizowanie plików programu SharePoint z nowym klientem synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9e0e8-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="9e0e8-120">Aby uzyskać więcej informacji, zapoznaj się z artykułem [Jak korzystać z polecenia "Otwórz z Eksploratorem", aby rozwiązać problemy w usłudze SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="9e0e8-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

