---
title: Przenoszenie wiadomości e-mail do archiwum Skrzynka pocztowa
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799790"
---
# <a name="move-email-to-the-archive-mailbox"></a>Przenoszenie wiadomości e-mail do archiwum Skrzynka pocztowa

Jeśli chcesz, aby w przypadku uruchamiania zautomatyzowanego sprawdzania ustawień wymienionych poniżej wybrać przycisk Wstecz <--u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z przenoszeniem wiadomości e-mail do ich archiwum.

1. Potwierdź, że włączono **skrzynkę pocztową archiwum** . Jeśli nie, wykonaj czynności opisane w [tym artykule](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , aby włączyć archiwizowaną skrzynkę pocztową.

2. Aby automatycznie archiwizować wiadomości w archiwum Skrzynka pocztowa, należy ustawić znacznik przechowywania z akcją **Przenieś do archiwum** , aby był **stosowany automatycznie do całego znacznika skrzynki pocztowej (domyślnego)**. Wykonaj poniższe czynności, aby utworzyć Tag: [archiwum domyślne](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Następnie Dodaj tag **archiwum** do zasad przechowywania. W centrum administracyjnym programu Exchange wybierz pozycję **zasady przechowywania** > Dodaj **tag Przenieś do archiwum** do zasad > **Zapisz**.

4. Teraz [Przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika. Te same zasady zostaną zastosowane zarówno do **głównej** , jak i do **archiwum** Skrzynka pocztowa.

Może być konieczne wymuszenie uruchomienia Asystenta zarządzanego folderu (MFA) i zastosowania nowych ustawień do skrzynki pocztowej użytkownika. Uruchom następujące polecenie podczas [nawiązania połączenia z programem EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Aby uzyskać więcej informacji na temat konfigurowania zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania dla skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  