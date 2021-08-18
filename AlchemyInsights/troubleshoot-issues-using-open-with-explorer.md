---
title: Rozwiązywanie problemów przy użyciu funkcji Otwórz w Eksploratorze
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323576"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rozwiązywanie problemów z otwieraniem w Eksploratorze

Rozwiązywanie typowych problemów z otwieraniem biblioteki dokumentów w programie SharePoint lub OneDrive przy użyciu polecenia Otwórz **w Eksploratorze:** 
  
- Użyj Internet Explorer 10 Lub Internet Explorer 11. **Otwórz w Eksploratorze** nie jest zgodny z przeglądarkami Microsoft Edge, Google Chrome, Firefox i innymi. **Ustawienia Otwórz w Eksploratorze** są wyłączone we wszystkich przeglądarkach oprócz programu Internet Explorer. 
    
- **Otwórz w Eksploratorze** nie jest dostępny w nowoczesnym środowisko obsługi dla SharePoint bibliotek. Zamiast **tego użyj widoku w Eksploratorze** plików. Wybierz **pozycję Opcje** \> **wyświetlania Wyświetl w Eksploratorze plików**. Wyświetlanie w Eksploratorze plików nie jest zgodne z przeglądarkami Microsoft Edge, Google Chrome, Firefox i innymi. **Wyświetl w Eksploratorze plików** w dostępne tylko w programie Internet Explorer. 
    
- Upewnij się, że usługa WebClient jest uruchomiona. W polu Windows wpisz uruchom, wybierz pozycję Uruchom aplikację komputerową, wpisz services.msc, a następnie naciśnij klawisz Enter. Przewiń w dół do usługi WebClient i upewnij się, że w **kolumnie Stan** jest wyświetlany tekst "Uruchomiony". Jeśli tak się nie stanie, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK.** (Najpierw może być konieczne włączenie usługi przez wybranie opcji **Ręcznie** lub Automatycznie **w** polu **Typ uruchomienia).** 
    
**Uwaga:** Otwarcie biblioteki w Eksploratorze plików jest przydatne, jeśli chcesz skopiować lub przenieść wiele plików i folderów jeden raz, ale jeśli chcesz regularnie pracować w bibliotece, zalecamy jej synchronizowanie. Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [Otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Aby uzyskać informacje na temat konfigurowania synchronizacji, zobacz SharePoint synchronizacji plików [za pomocą nowego synchronizacja usługi OneDrive klienta](https://go.microsoft.com/fwlink/?linkid=871666).
  
Aby uzyskać więcej informacji, zobacz artykuł Jak używać polecenia "Otwórz w Eksploratorze" w celu rozwiązywania problemów z usługą [SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

