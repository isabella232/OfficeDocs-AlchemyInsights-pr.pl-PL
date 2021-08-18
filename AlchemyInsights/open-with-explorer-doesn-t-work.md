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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321871"
---
# <a name="open-with-explorer-isnt-working"></a>Otwieranie w Eksploratorze nie działa

Jeśli ustawienie Otwórz  **w Eksploratorze** lub Wyświetl w Eksploratorze plików nie działa, upewnij się, że usługa WebClient została ustawiona na **Uruchomiona,** wykonać poniższe czynności. Na przykład otwarcie biblioteki usługi może zająć dużo czasu SharePoint lub OneDrive, gdy usługa nie jest uruchomiona. 
  
1. W polu Windows wpisz uruchom, wybierz pozycję Uruchom aplikację komputerową, wpisz services.msc, a następnie wybierz pozycję **Wprowadź**.
    
2. Przewiń w dół do usługi WebClient i sprawdź **kolumnę Stan.** Jeśli stan usługi WebClient nie ma stanu **Uruchomiony,** kliknij dwukrotnie usługę, kliknij pozycję **Uruchom,** a następnie kliknij przycisk **OK.** W razie potrzeby włącz usługę, wybierając opcję **Ręcznie** lub Automatycznie **w** polu **Typ uruchomienia.** 
    
**Uwaga:** Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Lepszym rozwiązaniem jest eksplorowanie synchronizacji: [synchronizowanie SharePoint plików za pomocą nowego synchronizacja usługi OneDrive klienta](https://go.microsoft.com/fwlink/?linkid=871666). 
  

