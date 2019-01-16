---
title: Otwórz w programie Explorer nie działa
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303857"
---
# <a name="open-with-explorer-isnt-working"></a>Otwórz w programie Explorer nie działa

Jeśli **Otwórz w Eksploratorze** lub **widoku w Eksploratorze plik** nie działa, upewnij się, że usługa WebClient jest ustawiona **uruchomiona** , wykonując poniższe kroki. Na przykład to może zająć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona. 
  
1. W polu wyszukiwania systemu Windows, typ uruchomienia, zaznacz aplikacji desktop Uruchom, wpisz services.msc i następnie wybierz **Enter**.
    
2. Przewiń w dół do usługi WebClient, a w kolumnie **Stan** . Jeśli stan usługi WebClient nie jest **uruchomiona**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij **OK**. Włącz usługę, jeśli to konieczne, przez wybranie w polu **Typ uruchomienia** **Ręczny** lub **Automatyczny** . 
    
> [!NOTE]
> Rozwiązywać problemy z otwieraniem w Eksploratorze plików, zobacz temat [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Poznaj synchronizacji jako lepsza alternatywa: [pliki programu SharePoint synchronizacji z nowym klientem synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

