---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900891"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rozwiązywanie problemów z udostępniania zawartości programu SharePoint dla użytkowników zewnętrznych

Upewnij się, że udostępniania zewnętrznych jest włączona dla organizacji:
  
1. Przejdź do [usług &amp; stronę dodatki w Centrum administracyjnym usługi Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknij przycisk **witryny**.
    
2. Upewnij się, że włączono ustawienie na "On". Jeśli zaznaczone jest "Tylko istniejących użytkowników zewnętrznych", upewnij się, zewnętrzne użytkownik jest wyświetlany w Centrum administracyjnym usługi Office 365.
    
Upewnij się, udostępniania zewnętrznych włączone dla witryny. Dla zbioru witryn klasyczne:
  
1. W klasycznym Centrum administracyjnego programu SharePoint, w lewym okienku kliknij **zbiorów witryn**.
    
2. Wybierz witrynę lub witryny, a na wstążce kliknij polecenie **Udostępnianie**.
    
Dla witryny zespołu, który należy do grupy usługi Office 365, lub witryny komunikacji:
  
- Te nowe typy witryny mają sam ustawienie udostępniania ustawienie całej organizacji, chyba że ustawienie całej organizacji pozwala na udostępnianie plików przy użyciu łącza, które nie wymagają rejestrowania. W takim przypadku witryn Zezwalaj na współużytkowanie z nowych i istniejących użytkowników zewnętrznych, którzy Zaloguj się. Aby zmienić ustawienie dla określonych witryn, należy użyć nowego Centrum administracyjnego programu SharePoint (Podgląd) lub programu PowerShell. [Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Ustawienia udostępniania zewnętrznych dla dowolnej witryny mogą być bardziej restrykcyjne niż ustawienia całej organizacji, ale nie bardziej liberalne niż ustawienie całej organizacji. 
  

