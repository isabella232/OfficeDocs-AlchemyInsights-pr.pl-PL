---
title: Rozwiązywanie problemów przy użyciu aplikacji Open with Explorer
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
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659068"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="0ae1c-102">Rozwiązywanie problemów dotyczących otwierania za pomocą Eksploratora</span><span class="sxs-lookup"><span data-stu-id="0ae1c-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="0ae1c-103">Rozwiązywanie typowych problemów dotyczących otwierania biblioteki dokumentów w programie SharePoint lub usłudze OneDrive przy użyciu polecenia **Otwórz za pomocą Eksploratora** :</span><span class="sxs-lookup"><span data-stu-id="0ae1c-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="0ae1c-104">Użyj programu Internet Explorer 10 lub Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="0ae1c-105">**Polecenie Otwórz w Eksploratorze** nie jest zgodne z aplikacją Microsoft Edge, Google Chrome, Firefox ani innymi.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0ae1c-106">Opcja **Otwórz w Eksploratorze** jest wyłączona we wszystkich przeglądarkach oprócz programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="0ae1c-107">**Otwieranie za pomocą Eksploratora** nie jest dostępne w nowoczesnych doświadczeniach dotyczących bibliotek programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="0ae1c-108">Zamiast tego użyj **widoku w Eksploratorze plików** .</span><span class="sxs-lookup"><span data-stu-id="0ae1c-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="0ae1c-109">Wybierz pozycję Widok **opcji widoku** \> **w Eksploratorze plików**.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="0ae1c-110">Widok w Eksploratorze plików nie jest zgodny z programem Microsoft Edge, Google Chrome, Firefox ani innymi.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="0ae1c-111">**Widok dostępne w Eksploratorze plików** jest dostępny tylko w programie Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="0ae1c-112">Upewnij się, że jest uruchomiona usługa WebClient.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="0ae1c-113">W polu wyszukiwania systemu Windows wpisz tekst Uruchom, zaznacz pozycję Uruchom aplikację klasyczną, wpisz Services. msc, a następnie naciśnij klawisz ENTER.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="0ae1c-114">Przewiń w dół do usługi WebClient i upewnij się, że w kolumnie **stan** jest wyświetlana wartość "uruchomiony".</span><span class="sxs-lookup"><span data-stu-id="0ae1c-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="0ae1c-115">Jeśli nie, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="0ae1c-116">(Być może musisz najpierw włączyć tę usługę, wybierając **ręcznie** lub **automatycznie** w polu **Typ uruchomienia** ).</span><span class="sxs-lookup"><span data-stu-id="0ae1c-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="0ae1c-117">Otwarcie biblioteki w Eksploratorze plików jest przydatne, jeśli trzeba raz skopiować lub przenieść wiele plików i folderów, ale jeśli chcesz regularnie pracować w bibliotece, zalecamy jej zsynchronizowanie.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="0ae1c-118">Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="0ae1c-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="0ae1c-119">Aby uzyskać informacje na temat konfigurowania synchronizacji, zobacz [synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="0ae1c-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="0ae1c-120">Zapoznaj się z artykułem [jak użyć polecenia "Otwórz w Eksploratorze", aby rozwiązać problemy w usłudze SharePoint Online,](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) Aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="0ae1c-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

