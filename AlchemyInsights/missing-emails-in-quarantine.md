---
title: Brakujące wiadomości e-mail w kwarantannie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569555"
---
# <a name="missing-emails-in-quarantine"></a>Brakujące e-maile w kwarantannie"

Administratorzy mogą [wyświetlać, zwalniać lub usuwać te wiadomości.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Aby otworzyć Centrum zgodności & zabezpieczeń, przejdź do pliku [https://protection.office.com](https://protection.office.com/) . Aby otworzyć stronę kwarantanny bezpośrednio, przejdź do [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Można wyszukiwać według następujących wartości:  

- **Identyfikator wiadomości:** globalnie unikatowy identyfikator wiadomości. Jeśli wybierzesz wiadomość na liście, w wyświetlonym okienku wysuwu **szczegółów** pojawi się wartość **identyfikatora wiadomości.** Administratorzy mogą używać [śledzenia wiadomości](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) do znajdowania wiadomości i odpowiadających im wartości identyfikatora wiadomości.
- **Adres e-mail nadawcy:** adres e-mail pojedynczego nadawcy.
- **Adres e-mail odbiorcy:** adres e-mail jednego adresata.
- **Temat**: Użyj całego tematu wiadomości. W wyszukiwaniu nie jest rozróżniana wielkość liter.

Po wprowadzeniu kryteriów wyszukiwania kliknij przycisk Odśwież przycisk ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Odśwież,** aby filtrować wyniki.  

Polecenia cmdlet używane do wyświetlania wiadomości i plików w kwarantannie oraz zarządzanie nimi to:
- [Usuń-KwarantannaMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksport-KwarantannaNajedzaj](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Pobierz kwarantannęSeułka](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Należy pamiętać, że to polecenie cmdlet jest przeznaczone tylko dla wiadomości, a nie plików złośliwego oprogramowania z usługi ATP dla usługi SharePoint Online, OneDrive dla Firm lub Zespołów.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)