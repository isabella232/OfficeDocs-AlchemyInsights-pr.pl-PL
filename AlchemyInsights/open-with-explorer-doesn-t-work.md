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
# <a name="open-with-explorer-isnt-working"></a>Otwieranie w Eksploratorze nie działa

Jeśli **otwarta za pomocą Eksploratora** lub **widoku w Eksploratorze plików** nie działa, upewnij się, że usługa WebClient jest skonfigurowana do **działania** , wykonując poniższe czynności. Na przykład otwarcie biblioteki programu SharePoint lub usługi OneDrive może zająć dużo czasu, gdy usługa nie jest uruchomiona. 
  
1. W polu wyszukiwania systemu Windows wpisz tekst Uruchom, zaznacz pozycję Uruchom aplikację klasyczną, wpisz Services. msc, a następnie wybierz pozycję **Enter**.
    
2. Przewiń w dół do usługi WebClient i Sprawdź kolumnę **stan** . Jeśli stan usługi WebClient nie jest **uruchomiony**, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**. W razie potrzeby Włącz usługę, wybierając opcję **ręcznie** lub **automatycznie** w polu **Typ uruchomienia** . 
    
> [!NOTE]
> Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Eksploruj synchronizację jako lepszą, alternatywną: [synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

