---
title: Otwieranie za pomocą Eksploratora nie działa
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694466"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="57312-102">Otwieranie w Eksploratorze nie działa</span><span class="sxs-lookup"><span data-stu-id="57312-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="57312-103">Jeśli **otwarta za pomocą Eksploratora** lub **widoku w Eksploratorze plików** nie działa, upewnij się, że usługa WebClient jest skonfigurowana do **działania** , wykonując poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="57312-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="57312-104">Na przykład otwarcie biblioteki programu SharePoint lub usługi OneDrive może zająć dużo czasu, gdy usługa nie jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="57312-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="57312-105">W polu wyszukiwania systemu Windows wpisz tekst Uruchom, zaznacz pozycję Uruchom aplikację klasyczną, wpisz Services. msc, a następnie wybierz pozycję **Enter**.</span><span class="sxs-lookup"><span data-stu-id="57312-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="57312-106">Przewiń w dół do usługi WebClient i Sprawdź kolumnę **stan** .</span><span class="sxs-lookup"><span data-stu-id="57312-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="57312-107">Jeśli stan usługi WebClient nie jest **uruchomiony**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="57312-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="57312-108">W razie potrzeby Włącz usługę, wybierając opcję **ręcznie** lub **automatycznie** w polu **Typ uruchomienia** .</span><span class="sxs-lookup"><span data-stu-id="57312-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="57312-109">Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="57312-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="57312-110">Eksploruj synchronizację jako lepszą, alternatywną: [synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="57312-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

