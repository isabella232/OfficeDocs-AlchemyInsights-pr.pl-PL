---
title: Przenoszenie wiadomości e-mail do skrzynki pocztowej archiwum
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660393"
---
Występują problemy podczas archiwizacji elementów do archiwum skrzynki pocztowej. Upewnij się, że zostały wykonane następujące czynności:
  
1. Upewnij się, że **archiwum skrzynki pocztowej** zostało włączone. Jeśli tak nie jest, wykonaj kroki w [tym artykule](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , aby umożliwić archiwum skrzynki pocztowej. 
    
2. W Centrum administracyjnego programu Exchange wybierz **Tagi przechowywania** w obszarze **Compliance Management**, Utwórz **tag przechowywania** z akcją **Przenieś do archiwum** zawierające żądane **Limitu czasowego**.
    
3. W Centrum administracyjnego programu Exchange wybierz **Zasady przechowywania**, utworzyć **Zasady przechowywania** i dodać tag przechowywania **Przenieś do archiwum** do tej zasady. 
    
4. [Przypisywanie zasad przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej danego użytkownika. Takie same zasady zostaną zastosowane do **podstawowego** i **archiwum** skrzynki pocztowej. 
    
Skrzynka pocztowa użytkownika powinny być zasad archiwizacji Aby przenieść elementy do archiwum skrzynki pocztowej. Może być konieczne wymuszenie zarządzanych folderów Asystenta (MFA) do uruchomienia i Zastosuj nowe ustawienia do skrzynki pocztowej danego użytkownika. Uruchom następujące polecenie podczas [podłączony do środowiska PowerShell EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Chcesz uzyskać więcej informacji na temat definiowania zasad archiwizacji, zobacz temat [Set up to archiwum i usuwanie zasady dla skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

