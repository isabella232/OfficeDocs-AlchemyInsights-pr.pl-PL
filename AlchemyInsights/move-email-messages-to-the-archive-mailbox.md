---
title: Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822172"
---
# <a name="move-email-to-the-archive-mailbox"></a>Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej

1. Potwierdź, że została włączona **archiwalna skrzynka pocztowa** . Jeśli nie, wykonaj kroki opisane w [tym artykule](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , aby włączyć archiwalną skrzynkę pocztową.

2. Aby automatycznie archiwizować wiadomości w archiwalnej skrzynce pocztowej, znacznik przechowywania z akcją **Przenieś na archiwizację** musi być ustawiony na **automatycznie zastosowany do całej skrzynki pocztowej (domyślnie)**. Wykonaj poniższe kroki, aby utworzyć znacznik: [Archive default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Następnie Dodaj tag **archiwum** do zasad przechowywania. W centrum administracyjnego programu Exchange wybierz **zasady przechowywania** > Dodaj **Przenieś do archiwum tag** do zasady > **Zapisz**.

4. Teraz [Przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika. Te same zasady zostaną zastosowane zarówno do **podstawowej** , jak i **archiwalnej** skrzynki pocztowej.

Może być konieczne wymuszenie Asystenta folderów zarządzanych (MFA), aby uruchomić i zastosować nowe ustawienia do skrzynki pocztowej użytkownika. Uruchom następujące polecenie podczas [połączenia z EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:
  
Start-ManagedFolderAssistant-tożsamość<name of the mailbox>

Aby uzyskać więcej informacji o konfigurowaniu zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania dla skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  