---
title: Zasady przechowywania w Centrum administracyjnego programu Exchange nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371308"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zasady przechowywania w Centrum administracyjnego programu Exchange

 **Problem:** Nowo utworzony lub zasady przechowywania zaktualizowane w Centrum administracyjnego programu Exchange nie są stosowane do skrzynek pocztowych lub elementy nie są przenoszone do archiwum skrzynki pocztowej lub usunięte. 
  
 **Główne przyczyny:**
  
- Może to być spowodowane **Zarządzany Asystent folderów** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych próbuje przetworzyć każdą skrzynkę pocztową w organizacji chmurze co siedem dni. Jeśli zmianie tagu przechowywania lub zastosowania innych zasad przechowywania do skrzynki pocztowej, możesz poczekać aż zarządzanych folderów pomagają przetwarza skrzynki pocztowej, lub można uruchomić polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych do przetwarzania określonego Skrzynka pocztowa. Uruchomienie tego polecenia cmdlet jest użyteczne dla testowania i rozwiązywania problemów z zasad przechowywania lub ustawienia znacznika przechowywania. Aby uzyskać więcej informacji odwiedź witrynę [uruchomić Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rozwiązania:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To również może wystąpić, jeśli **RetentionHold** została **włączona** do skrzynki pocztowej. Jeśli skrzynka pocztowa jest umieszczone na RetentionHold, zasad przechowywania do skrzynki pocztowej nie będą przetwarzane w tym czasie. Aby uzyskać więcej informacji, zobacz ustawienie RetentionHold: [Przytrzymaj przechowywania skrzynki pocztowej](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rozwiązanie:**
    
  - Sprawdź ustawienie RetentionHold określonej skrzynki pocztowej w [programie powershell EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Uruchom następujące polecenie, aby **wyłączyć** RetentionHold na określonej skrzynki pocztowej: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz uruchom ponownie folder zarządzany Asystent:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Uwaga:** Jeśli skrzynka pocztowa jest mniejszy niż 10 MB, zarządzany Asystent folderów nie będzie automatycznie przetwarzać skrzynki pocztowej. 
  

