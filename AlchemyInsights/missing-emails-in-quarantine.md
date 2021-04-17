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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831744"
---
# <a name="missing-emails-in-quarantine"></a>Brakujące wiadomości e-mail w kwarantannie"

Administratorzy [mogą wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do [https://protection.office.com](https://protection.office.com/) . Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) strony .  

Możesz wyszukiwać według następujących wartości:  

- **Identyfikator wiadomości:** unikatowy identyfikator globalny wiadomości. Jeśli wybierzesz wiadomość na liście, wartość Identyfikator wiadomości zostanie wyświetlona w  **wyświetlonym okienku wysuwu** Szczegóły. Administratorzy mogą za [pomocą funkcji śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) znaleźć wiadomości i odpowiadające im wartości identyfikatora wiadomości.
- **Adres e-mail nadawcy:** adres e-mail jednego nadawcy.
- **Adres e-mail adresata:** adres e-mail pojedynczego adresata.
- **Temat:** użyj całego tematu wiadomości. W wyszukiwaniu nie jest wróżniana wielkość liter.

Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież, aby ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  przefiltrować wyniki.  

Polecenia cmdlet, których używasz do wyświetlania wiadomości i plików w kwarantannie oraz zarządzania nimi w kwarantannie, to:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Pamiętaj, że to polecenie cmdlet jest tylko dla wiadomości, a nie plików złośliwego oprogramowania z atp dla usługi SharePoint Online, OneDrive dla Firm lub Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)