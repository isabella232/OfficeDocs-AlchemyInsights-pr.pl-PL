---
title: Otwieranie za pomocą Eksploratora nie działa
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713044"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="2a1f7-102">Otwórz za pomocą Eksploratora nie działa</span><span class="sxs-lookup"><span data-stu-id="2a1f7-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="2a1f7-103">Jeśli **otwórz za pomocą Eksploratora** lub Wyświetl w **Eksploratorze plików** nie działa, upewnij się, że usługa WebClient jest ustawiona na **Uruchomiona,** wykonując poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="2a1f7-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="2a1f7-104">Na przykład może upłynąć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona.</span><span class="sxs-lookup"><span data-stu-id="2a1f7-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="2a1f7-105">W polu wyszukiwania systemu Windows wpisz polecenie Uruchom aplikację klasyczną, wpisz services.msc, a następnie wybierz pozycję **Enter**.</span><span class="sxs-lookup"><span data-stu-id="2a1f7-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="2a1f7-106">Przewiń w dół do usługi WebClient i sprawdź kolumnę **Stan.**</span><span class="sxs-lookup"><span data-stu-id="2a1f7-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="2a1f7-107">Jeśli stan usługi WebClient nie jest **uruchomiony,** kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="2a1f7-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2a1f7-108">Włącz usługę, jeśli to konieczne, wybierając opcję **Ręczny** lub **Automatyczny** w polu **Typ uruchamiania.**</span><span class="sxs-lookup"><span data-stu-id="2a1f7-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2a1f7-109">Aby rozwiązać problemy z otwieraniem się w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2a1f7-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2a1f7-110">Eksploruj synchronizację jako lepszą alternatywę: [synchronizuj pliki programu SharePoint z nowym klientem synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2a1f7-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

