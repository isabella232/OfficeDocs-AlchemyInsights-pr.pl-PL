---
title: Zasady przechowywania w centrum administracyjnym programu Exchange nie działają
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740520"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zasady przechowywania w centrum administracyjnym programu Exchange

Jeśli chcesz, aby w przypadku uruchamiania zautomatyzowanej kontroli nad ustawieniami wymienionymi poniżej, wybierz przycisk Wstecz <--u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z zasadami przechowywania.

 **Problem:** Nowo utworzone lub zaktualizowane zasady przechowywania w centrum administracyjnym programu Exchange nie są stosowane do skrzynek pocztowych ani elementów, które nie są przenoszone do archiwum ani do usuniętej archiwalnej skrzynki pocztowej. 
  
 **Główne przyczyny:**
  
- Może to wynikać z faktu, że **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych próbuje przetwarzać każdą skrzynkę pocztową w organizacji opartą na chmurze raz na siedem dni. Jeśli zmienisz znacznik przechowywania lub zastosowano inne zasady przechowywania do skrzynki pocztowej, możesz poczekać, aż folder zarządzany będzie mógł przetworzyć skrzynkę pocztową, lub uruchomić polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych w celu przetworzenia określonej skrzynki pocztowej. Uruchomienie tego polecenia cmdlet jest przydatne w przypadku testowania lub rozwiązywania problemów dotyczących zasad przechowywania lub ustawień znaczników przechowywania. Aby uzyskać więcej informacji, odwiedź stronę [uruchamianie Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rozwiązanie:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Może to być również możliwe, jeśli w skrzynce pocztowej **włączono** **RetentionHold** . Jeśli skrzynka pocztowa została umieszczona na RetentionHoldie, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie. Aby uzyskać więcej Informaton na temat ustawienia RetentionHold, zobacz: [Blokada przechowywania skrzynek pocztowych](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rozwiązać**
    
  - Sprawdź stan ustawienia RetentionHold w określonej skrzynce pocztowej w programie [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Uruchom następujące polecenie, aby **wyłączyć** RetentionHold w określonej skrzynce pocztowej:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz uruchom ponownie Asystenta zarządzanego folderu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzać skrzynki pocztowej.
 
Aby uzyskać więcej informacji na temat zasad przechowywania w centrum administracyjnym programu Exchange, zobacz:
- [Tagi przechowywania i zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Stosowanie zasad przechowywania do skrzynek pocztowych](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodawanie lub usuwanie znaczników przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Jak zidentyfikować typ blokady umieszczanej w skrzynce pocztowej](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
