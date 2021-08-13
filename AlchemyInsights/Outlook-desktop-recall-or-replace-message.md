---
title: Outlook Odwoływanie lub zamienianie wiadomości e-mail na pulpicie
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918405"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odwoływanie lub zamienianie Outlook-mail

- Jako administrator możesz odwołać wiadomości w imieniu użytkowników **za pomocą programu PowerShell.** Nie można odwołać wiadomości z centrum administracyjnego.
- Odwoływanie **wiadomości wysyłanych do osób w organizacji** jest możliwe tylko. Jeśli na przykład wiadomość została wysłana na adres usługi Gmail, nie można jej odwołać.
- Możesz **odwołać tylko wiadomości wysłane z Outlook 2016 na komputerze.** Jeśli użytkownik wyśle wiadomość przy Outlook dla komputerów Mac lub Outlook w sieci Web, nie można jej odwołać.

Aby odwołać lub zamienić wiadomość e-mail:

1. W okienku folderów po lewej stronie Outlook wybierz folder Elementy wysłane.
1. Kliknij dwukrotnie wiadomość, którą chcesz odwołać, aby ją otworzyć.
1. Wybierz **kartę Wiadomość,** a następnie wybierz **pozycję Akcje**  >  **Odwołaj tę wiadomość.**
1. Wybierz **pozycję Usuń nieprzeczytane kopie** tej wiadomości lub Usuń **nieprzeczytane kopie** i zamień je na nową wiadomość, a następnie wybierz przycisk **OK.**
1. Jeśli wysyłasz wiadomość zastępczą, zredagotuj ją, a następnie wybierz pozycję **Wyślij**.
1. Skuteczność odwołania wiadomości lub jej niepowodzenia zależy od ustawień adresata w programie Outlook. Instrukcje sprawdzania odwołania można znaleźć w [tym artykule.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

- Jeśli nie jesteś administratorem globalnym, aby wyszukiwać wiadomości, Twoje konto musi być dodane do roli Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwaniem zgodności. Aby usunąć wiadomości, musisz dołączyć do grupy ról Zarządzanie organizacją lub do roli zarządzania wyszukiwaniem i przeczyszczanie. Uprawnienia do tych ról są przypisywane w [Centrum zabezpieczeń i zgodności.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/microsoft-365/compliance/content-search) aby znaleźć wiadomość do usunięcia.
- [Połączenie do Centrum zabezpieczeń i zgodności programu PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz Połączenie, Microsoft 365 centrum zabezpieczeń i zgodności programu PowerShell przy użyciu uwierzytelniania [wieloskładnikowego.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)