---
title: Brak przepływu pracy nie można aktywować
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052623"
---
# <a name="missing-workflow-failed-to-activate"></a>Brak przepływu pracy nie można aktywować

W zbiorze witryn programu Microsoft SharePoint nie można dodać globalnego przepływu pracy wielokrotnego użytku (na przykład "zatwierdzanie-SharePoint 2010") do listy lub biblioteki.
  
Aby rozwiązać ten problem, wykonaj następujące kroki: 
  
1. Otwórz stronę główną witryny sieci Web zbioru witryn w programie SharePoint Designer 2013.
  
2. W obszarze **obiekty lokacji**wybierz pozycję **przepływy pracy**. 
  
3. W **Nowa** sekcja na Wstążce **przepływy pracy** , wybierz **przepływu pracy wielokrotnego użytku**. 
  
4. W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** wprowadź nazwę * * *Repair2010* * *. Dla **typu platformy**, kliknij przycisk **przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**. 
  
1. W **Zapisz** sekcji na Wstążce **przepływu pracy** , wybierz **publikowania**. 
  
2. W sekcji **Zarządzaj** na Wstążce **przepływu pracy** wybierz **publikowania globalnie**. W wyświetlonym oknie dialogowym potwierdzenia wybierz **przycisk OK**. 
  
3. W przeglądarce sieci Web zlokalizuj głównej witryny sieci Web zbioru witryn, a następnie dostęp do \> **funkcji zbioru witryn** **Ustawienia witryny** . Następnie Przełącz funkcję **przepływy pracy** : 
  
· Jeśli funkcja jest *aktywna* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Aktywuj**. 
  
· Jeśli funkcja jest *dezaktywowana* , kliknij przycisk **Aktywuj**. 
  
Aby uzyskać więcej informacji, zapoznaj się z następującym [artykułem](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

