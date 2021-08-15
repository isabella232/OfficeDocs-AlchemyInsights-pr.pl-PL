---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026232"
---
# <a name="missing-emails-in-quarantine"></a>Brakujące wiadomości e-mail w kwarantannie"

Administratorzy [mogą wyświetlać, zwalniać lub usuwać te wiadomości.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do [https://protection.office.com](https://protection.office.com/) . Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) strony .  

Możesz wyszukiwać według następujących wartości:  

- **Identyfikator wiadomości:** unikatowy identyfikator globalny wiadomości. Jeśli wybierzesz wiadomość na liście, wartość Identyfikator wiadomości zostanie wyświetlona w  **wyświetlonym okienku wysuwu** Szczegóły. Administratorzy mogą za [pomocą funkcji śledzenia wiadomości](/microsoft-365/security/office-365-security/message-trace-scc) znaleźć wiadomości i odpowiadające im wartości identyfikatora wiadomości.
- **Adres e-mail nadawcy:** adres e-mail jednego nadawcy.
- **Adres e-mail adresata:** adres e-mail pojedynczego adresata.
- **Temat:** użyj całego tematu wiadomości. W wyszukiwaniu nie jest wróżniana wielkość liter.

Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież, aby ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  przefiltrować wyniki.

Polecenia cmdlet, których używasz do wyświetlania wiadomości i plików w kwarantannie oraz zarządzania nimi w kwarantannie, to:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)To polecenie cmdlet jest tylko dla wiadomości, a nie plików złośliwego oprogramowania z programu Microsoft Defender dla usługi Office 365 dla usługi SharePoint Online, OneDrive dla Firm lub Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)