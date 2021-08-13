---
title: Przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974967"
---
# <a name="move-email-to-the-archive-mailbox"></a>Przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej

Jeśli chcesz, abyśmy uruchamiali automatyczne testy ustawień wymienionych poniżej, wybierz przycisk wstecz < — u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z przenoszeniem poczty e-mail do jego archiwaowej skrzynki pocztowej.

1. Upewnij się, że **archiwizowa skrzynka pocztowa** została włączona. W innym przypadku należy wykonać czynności opisane w [tym artykule,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) aby włączyć archiwalne skrzynki pocztowe.

2. Aby wiadomości zarchiwizować automatycznie w  archiwaowej skrzynce pocztowej, należy ustawić tag przechowywania z akcją Przenieś do archiwum, który ma być stosowany automatycznie do całego **tagu skrzynki pocztowej (domyślny).** Aby utworzyć tag, skorzystaj z procedury opisanej w tym miejscu: Tag domyślny [archiwizacji](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Następnie dodaj tag **Archiwum** do zasad przechowywania. W centrum Exchange administracyjnego wybierz pozycję Zasady **przechowywania>** aby dodać **tag** Przenieś do archiwum do > **Zapisz.**

4. Teraz [przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika. Te same zasady zostaną zastosowane zarówno do skrzynki **pocztowej podstawowej,** jak **i** archiwaowej.

Może być konieczne wymusze na asystencie folderów zarządzanych (MFA) uruchomienie i zastosowanie nowych ustawień do skrzynki pocztowej użytkownika. Uruchom następujące polecenie podczas połączenia [z programem PowerShell programu EXO,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aby uruchomić asystenta folderów zarządzanych dla konkretnej skrzynki pocztowej:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Aby uzyskać więcej informacji na temat konfigurowania zasad archiwizacji, zobacz Konfigurowanie zasad archiwizacji i usuwania [dla skrzynek pocztowych.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  