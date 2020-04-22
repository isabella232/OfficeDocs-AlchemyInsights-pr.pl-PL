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
# <a name="open-with-explorer-isnt-working"></a>Otwórz za pomocą Eksploratora nie działa

Jeśli **otwórz za pomocą Eksploratora** lub Wyświetl w **Eksploratorze plików** nie działa, upewnij się, że usługa WebClient jest ustawiona na **Uruchomiona,** wykonując poniższe kroki. Na przykład może upłynąć dużo czasu, aby otworzyć bibliotekę programu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona. 
  
1. W polu wyszukiwania systemu Windows wpisz polecenie Uruchom aplikację klasyczną, wpisz services.msc, a następnie wybierz pozycję **Enter**.
    
2. Przewiń w dół do usługi WebClient i sprawdź kolumnę **Stan.** Jeśli stan usługi WebClient nie jest **uruchomiony,** kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**. Włącz usługę, jeśli to konieczne, wybierając opcję **Ręczny** lub **Automatyczny** w polu **Typ uruchamiania.** 
    
> [!NOTE]
> Aby rozwiązać problemy z otwieraniem się w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Eksploruj synchronizację jako lepszą alternatywę: [synchronizuj pliki programu SharePoint z nowym klientem synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

