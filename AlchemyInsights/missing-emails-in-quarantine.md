---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673724"
---
# <a name="missing-emails-in-quarantine"></a>Brakujące wiadomości e-mail w kwarantannie

Administratorzy mogą [wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Aby otworzyć Centrum zabezpieczeń & zgodności, przejdź do [https://protection.office.com](https://protection.office.com/) . Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do strony [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Możesz wyszukiwać według następujących wartości:  

- **Identyfikator wiadomości**: unikatowy identyfikator globalny wiadomości. Po zaznaczeniu wiadomości na liście zostanie wyświetlona wartość  **identyfikatora wiadomości**  w wyświetlonym okienku menu wysuwanego  **szczegóły**  . Administratorzy mogą używać [funkcji śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) do znajdowania wiadomości i ich odpowiednich wartości identyfikatorów wiadomości.
- **Adres E-mail nadawcy**: adres e-mail jednego nadawcy.
- **Adres E-mail adresata**: adres e-mail jednego adresata.
- **Temat**: Użyj całego tematu wiadomości. W wyszukiwaniu wielkość liter nie jest uwzględniana.

Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk ![ Odśwież ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Odśwież** , aby przefiltrować wyniki.  

Polecenia cmdlet służące do wyświetlania i zarządzania wiadomościami oraz plikami w kwarantannie są następujące:
- [DELETE-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksportowanie — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Wersja Preview — QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Zauważ, że to polecenie cmdlet jest przeznaczone tylko dla wiadomości, a nie do plików złośliwego oprogramowania w usłudze SharePoint Online, OneDrive dla firm lub w usłudze Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)