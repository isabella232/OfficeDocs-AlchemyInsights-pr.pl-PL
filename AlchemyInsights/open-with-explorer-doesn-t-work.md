---
title: Otwórz w programie Explorer nie działa
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906814"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="01485-102">Otwórz w programie Explorer nie działa</span><span class="sxs-lookup"><span data-stu-id="01485-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="01485-p101">Jeśli **Otwórz w Eksploratorze** lub **widoku w Eksploratorze plik** nie działa, upewnij się, że usługa WebClient jest ustawiona **uruchomiona** , wykonując poniższe kroki. Na przykład to może zająć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="01485-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="01485-105">W polu wyszukiwania systemu Windows, typ uruchomienia, zaznacz aplikacji desktop Uruchom, wpisz services.msc i następnie wybierz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="01485-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="01485-p102">Przewiń w dół do usługi WebClient, a w kolumnie **Stan** . Jeśli stan usługi WebClient nie jest **uruchomiona**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij **OK**. Włącz usługę, jeśli to konieczne, przez wybranie w polu **Typ uruchomienia** **Ręczny** lub **Automatyczny** .</span><span class="sxs-lookup"><span data-stu-id="01485-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="01485-p103">Rozwiązywać problemy z otwieraniem w Eksploratorze plików, zobacz temat [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Poznaj synchronizacji jako lepsza alternatywa: [pliki programu SharePoint synchronizacji z nowym klientem synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="01485-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

