---
title: Przenoszenie wiadomości e-mail do skrzynki pocztowej Archiwum
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511050"
---
# <a name="move-email-to-the-archive-mailbox"></a>Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej

1. Upewnij się, że **skrzynka pocztowa archiwum** została włączona. Jeśli nie, użyj kroków w [tym artykule,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) aby włączyć archiwalnej skrzynki pocztowej.

2. Aby automatycznie archiwizować wiadomości do archiwalnej skrzynki pocztowej, tag przechowywania z akcją **Przenieś do archiwum** musi być automatycznie **stosowany do całego tagu skrzynki pocztowej (domyślnie).** Użyj kroków tutaj, aby utworzyć tag: [Archiwum domyślny tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Następnie dodaj tag **Archiwum** do zasad przechowywania. W Centrum administracyjnym programu Exchange wybierz pozycję **Zasady przechowywania** > dodaj tag Przenieś **do archiwum** do zasad > **Zapisz**.

4. Teraz [przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika. Ta sama zasada zostanie zastosowana zarówno do **skrzynki pocztowej Podstawowa,** jak i **Archiwum.**

Może być konieczne wymuszenie uruchomienia asystenta folderów zarządzanych (MFA) i zastosowania nowych ustawień do skrzynki pocztowej użytkownika. Uruchom następujące polecenie po [podłączeniu do programu EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:
  
Start-ManagedFolderAssistant -Tożsamość<name of the mailbox>

Aby uzyskać więcej informacji na temat konfigurowania zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  