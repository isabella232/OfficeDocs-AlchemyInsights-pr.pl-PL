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
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764918"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e913a-102">Otwórz w programie Explorer nie działa</span><span class="sxs-lookup"><span data-stu-id="e913a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e913a-103">Jeśli **Otwórz w Eksploratorze** lub **widoku w Eksploratorze plik** nie działa, upewnij się, że usługa WebClient jest ustawiona **uruchomiona** , wykonując poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="e913a-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="e913a-104">Na przykład to może zająć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="e913a-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e913a-105">W polu wyszukiwania systemu Windows, typ uruchomienia, zaznacz aplikacji desktop Uruchom, wpisz services.msc i następnie wybierz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e913a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e913a-106">Przewiń w dół do usługi WebClient, a w kolumnie **Stan** .</span><span class="sxs-lookup"><span data-stu-id="e913a-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="e913a-107">Jeśli stan usługi WebClient nie jest **uruchomiona**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij **OK**.</span><span class="sxs-lookup"><span data-stu-id="e913a-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e913a-108">Włącz usługę, jeśli to konieczne, przez wybranie w polu **Typ uruchomienia** **Ręczny** lub **Automatyczny** .</span><span class="sxs-lookup"><span data-stu-id="e913a-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e913a-109">Rozwiązywać problemy z otwieraniem w Eksploratorze plików, zobacz temat [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e913a-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e913a-110">Poznaj synchronizacji jako lepsza alternatywa: [pliki programu SharePoint synchronizacji z nowym klientem synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e913a-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

