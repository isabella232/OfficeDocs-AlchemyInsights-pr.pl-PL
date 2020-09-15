---
title: Nie można aktywować brakującego przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667096"
---
# <a name="missing-workflow-failed-to-activate"></a>Nie można aktywować brakującego przepływu pracy

W zbiorze witryn programu Microsoft SharePoint nie można dodać globalnego przepływu pracy do wielokrotnego użytku (takiego jak "zatwierdzanie — SharePoint 2010") do listy lub biblioteki.
  
Aby rozwiązać ten problem, wykonaj następujące czynności: 
  
1. Otwórz główną witrynę sieci Web zbioru witryn w programie SharePoint Designer 2013.
  
2. W obszarze **obiekty witryny**wybierz pozycję **przepływy pracy**. 
  
3. W **nowej** sekcji wstążki **przepływy pracy** wybierz pozycję **przepływ pracy wielokrotnego użytku**. 
  
4. W formularzu **Utwórz przepływ pracy wielokrotnego użytku** wprowadź nazwę * * *Repair2010* * *. W obszarze **Typ platformy**kliknij pozycję **przepływ pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**. 
  
1. W sekcji **Zapisywanie** wstążki **przepływu pracy** wybierz pozycję **Publikuj**. 
  
2. W sekcji **Zarządzanie** na Wstążce **przepływu pracy** wybierz pozycję **Publikuj globalnie**. W wyświetlonym oknie dialogowym potwierdzenia wybierz **przycisk OK**. 
  
3. W przeglądarce internetowej Znajdź główną witrynę sieci Web zbioru witryn, a następnie uzyskaj dostęp do **Site Settings** \> **funkcji zbioru witryn**ustawienia witryny. Następnie Przełącz funkcję **przepływy pracy** : 
  
· Jeśli funkcja jest  *aktywowana*  , kliknij pozycję **Dezaktywuj,** a następnie kliknij pozycję **Aktywuj**. 
  
· Jeśli funkcja jest  *wyłączona*  , kliknij pozycję **Aktywuj**. 
  
Więcej informacji znajdziesz w poniższym [artykule](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

