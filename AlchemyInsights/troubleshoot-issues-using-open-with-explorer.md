---
title: Rozwiązywanie problemów przy użyciu aplikacji Open with Explorer
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659068"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rozwiązywanie problemów dotyczących otwierania za pomocą Eksploratora

Rozwiązywanie typowych problemów dotyczących otwierania biblioteki dokumentów w programie SharePoint lub usłudze OneDrive przy użyciu polecenia **Otwórz za pomocą Eksploratora** : 
  
- Użyj programu Internet Explorer 10 lub Internet Explorer 11. **Polecenie Otwórz w Eksploratorze** nie jest zgodne z aplikacją Microsoft Edge, Google Chrome, Firefox ani innymi. Opcja **Otwórz w Eksploratorze** jest wyłączona we wszystkich przeglądarkach oprócz programu Internet Explorer. 
    
- **Otwieranie za pomocą Eksploratora** nie jest dostępne w nowoczesnych doświadczeniach dotyczących bibliotek programu SharePoint. Zamiast tego użyj **widoku w Eksploratorze plików** . Wybierz pozycję Widok **opcji widoku** \> **w Eksploratorze plików**. Widok w Eksploratorze plików nie jest zgodny z programem Microsoft Edge, Google Chrome, Firefox ani innymi. **Widok dostępne w Eksploratorze plików** jest dostępny tylko w programie Internet Explorer. 
    
- Upewnij się, że jest uruchomiona usługa WebClient. W polu wyszukiwania systemu Windows wpisz tekst Uruchom, zaznacz pozycję Uruchom aplikację klasyczną, wpisz Services. msc, a następnie naciśnij klawisz ENTER. Przewiń w dół do usługi WebClient i upewnij się, że w kolumnie **stan** jest wyświetlana wartość "uruchomiony". Jeśli nie, kliknij dwukrotnie usługę, kliknij przycisk **Start**, a następnie kliknij przycisk **OK**. (Być może musisz najpierw włączyć tę usługę, wybierając **ręcznie** lub **automatycznie** w polu **Typ uruchomienia** ). 
    
> [!NOTE]
> Otwarcie biblioteki w Eksploratorze plików jest przydatne, jeśli trzeba raz skopiować lub przenieść wiele plików i folderów, ale jeśli chcesz regularnie pracować w bibliotece, zalecamy jej zsynchronizowanie. Aby rozwiązać problemy z otwieraniem w Eksploratorze plików, zobacz [otwieranie w Eksploratorze](https://go.microsoft.com/fwlink/?linkid=871665). Aby uzyskać informacje na temat konfigurowania synchronizacji, zobacz [synchronizowanie plików programu SharePoint za pomocą nowego klienta synchronizacji usługi OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Zapoznaj się z artykułem [jak użyć polecenia "Otwórz w Eksploratorze", aby rozwiązać problemy w usłudze SharePoint Online,](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) Aby uzyskać więcej informacji. 
  

