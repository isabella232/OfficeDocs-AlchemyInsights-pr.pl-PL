---
title: Zasady przechowywania w Centrum administracyjnym programu Exchange nie działają
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742443"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zasady przechowywania w Centrum administracyjnym programu Exchange

 **Problem:** Nowo utworzone lub zaktualizowane zasady przechowywania w Centrum administracyjnym programu Exchange nie mają zastosowania do skrzynek pocztowych lub elementy nie są przenoszone do archiwalnej skrzynki pocztowej ani usuwane. 
  
 **Przyczyn:**
  
- Może to być spowodowane tym, że **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych próbuje przetworzyć każdą skrzynkę pocztową w organizacji chmurowej raz na siedem dni. Jeśli zmienisz tag przechowywania lub zastosujesz inną zasadę przechowywania do skrzynki pocztowej, możesz poczekać, aż Asysta folderu zarządzanego przetworzy skrzynkę pocztową lub uruchomisz polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych w celu przetworzenia określonej skrzynki pocztowej. Uruchamianie tego polecenia cmdlet jest przydatne do testowania lub rozwiązywania problemów z ustawieniami zasad przechowywania lub tagu przechowywania. Aby uzyskać więcej informacji, odwiedź stronę [Uruchom Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rozwiązanie:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Może to również wystąpić, jeśli **retentionHold** została **włączona** w skrzynce pocztowej. Jeśli skrzynka pocztowa została umieszczona w retencji, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie. Aby uzyskać więcej informacji na temat ustawienia HoldHold, zobacz: [Wstrzymanie przechowywania skrzynki pocztowej](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rozwiązanie:**
    
  - Sprawdź stan ustawienia Retencja w określonej skrzynce pocztowej w programie [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Uruchom następujące polecenie, aby **wyłączyć** retencję w określonej skrzynce pocztowej:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz ponownie uruchom Asystenta folderu zarządzanego:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzał skrzynki pocztowej.
 
Aby uzyskać więcej informacji na temat zasad przechowywania w Centrum administracyjnym programu Exchange, zobacz:
- [Tagi przechowywania i zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Stosowanie zasad przechowywania do skrzynek pocztowych](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodawanie lub usuwanie znaczników przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Jak zidentyfikować typ blokady umieszczonej na skrzynce pocztowej](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
