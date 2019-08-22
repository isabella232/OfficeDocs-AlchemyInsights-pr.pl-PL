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
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538492"
---
# <a name="open-with-explorer-isnt-working"></a>Otwórz w programie Explorer nie działa

Jeśli **Otwórz w Eksploratorze** lub **widoku w Eksploratorze plik** nie działa, upewnij się, że usługa WebClient jest ustawiona **uruchomiona** , wykonując poniższe kroki. Na przykład to może zająć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona. 
  
1. W polu wyszukiwania systemu Windows, typ uruchomienia, zaznacz aplikacji desktop Uruchom, wpisz services.msc i następnie wybierz **Enter**.
    
2. Przewiń w dół do usługi WebClient, a w kolumnie **Stan** . Jeśli stan usługi WebClient nie jest **uruchomiona**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij **OK**. Włącz usługę, jeśli to konieczne, przez wybranie w polu **Typ uruchomienia** **Ręczny** lub **Automatyczny** . 
    
> [!NOTE]
> Rozwiązywać problemy z otwieraniem w Eksploratorze plików, zobacz temat [Otwórz w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Poznaj synchronizacji jako lepsza alternatywa: [pliki programu SharePoint synchronizacji z nowym klientem synchronizacji OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

