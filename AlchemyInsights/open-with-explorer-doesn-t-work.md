---
title: Nie działa okno Otwórz w Eksploratorze
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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011346"
---
# <a name="open-with-explorer-isnt-working"></a>Otwieranie w Eksploratorze nie działa

Jeśli przycisk Otwórz  **w Eksploratorze** lub Wyświetl w Eksploratorze plików nie działa, upewnij się, że usługa WebClient została ustawiona na **Uruchomiona,** wykonać poniższe czynności. Na przykład otwarcie biblioteki danych lub biblioteki usługi może zająć dużo SharePoint lub biblioteki OneDrive, gdy usługa nie jest uruchomiona. 
  
1. W polu Windows wpisz uruchom, wybierz pozycję Uruchom aplikację komputerową, wpisz services.msc, a następnie wybierz pozycję **Wprowadź**.
    
2. Przewiń w dół do usługi WebClient i sprawdź **kolumnę Stan.** Jeśli stan usługi WebClient nie ma stanu **Uruchomiony,** kliknij dwukrotnie usługę, kliknij pozycję **Uruchom,** a następnie kliknij przycisk **OK.** W razie potrzeby włącz usługę, wybierając opcję **Ręcznie** lub Automatycznie **w** polu **Typ uruchomienia.** 
    
> [!NOTE]
> Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Lepszym rozwiązaniem jest eksplorowanie synchronizacji: [synchronizowanie SharePoint plikami za pomocą nowego synchronizacja usługi OneDrive klienta](https://go.microsoft.com/fwlink/?linkid=871666). 
  

