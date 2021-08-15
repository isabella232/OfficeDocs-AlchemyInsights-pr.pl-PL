---
title: Odwoływanie lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024396"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odwoływanie lub zamienianie wiadomości e-mail w programie Microsoft 365

- Odwoływanie **wiadomości wysyłanych do osób w organizacji** jest możliwe tylko. Jeśli na przykład wiadomość została wysłana na adres usługi Gmail, nie można jej odwołać.
- Możesz **odwołać tylko wiadomości** wysłane z Outlook na komputer. Jeśli użytkownik wyśle wiadomość przy Outlook dla komputerów Mac lub Outlook w sieci Web, nie można jej odwołać.
- Jako administrator dzierżawy, możesz odwołać wiadomości w **imieniu** użytkowników przy użyciu programu PowerShell (Aby uzyskać więcej informacji, zobacz: Wyszukiwanie i usuwanie wiadomości [e-mail).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Nie można odwołać wiadomości z centrum administracyjnego. Przewiń w dół do przycisku "Wyszukaj i usuń wiadomości e-mail w organizacji", aby uzyskać więcej informacji.

**Odwoływanie lub zamienianie wysłanej wiadomości e-mail**

1. W okienku folderów po lewej stronie Outlook wybierz folder Elementy wysłane.
2. Otwórz wiadomość, którą chcesz odwołać. Należy kliknąć dwukrotnie, aby otworzyć wiadomość. Zaznaczenie wiadomości w celu jej zaznaczenia w okienku odczytu nie umożliwia jej odwołania.
3. Na karcie Wiadomość wybierz pozycję **Akcje**  >  **odwołaj tę wiadomość.**
4. Wybierz **pozycję Usuń nieprzeczytane kopie** tej wiadomości lub Usuń **nieprzeczytane kopie** i zamień je na nową wiadomość , a następnie wybierz przycisk **OK.**
5. Jeśli wysyłasz wiadomość zastępczą, zredagotuj ją, a następnie wybierz pozycję **Wyślij**.
6. Skuteczność odwołania wiadomości jest uzależniona od ustawień adresata w programie Outlook.

Aby uzyskać więcej informacji, w tym na temat sprawdzania odwołania, zobacz Odwoływanie lub zamienianie wysłanej wiadomości [e-mail.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Jeśli chcesz wyszukiwać i usuwać*** wiadomości e-mail w organizacji, najłatwiej jest być administratorem globalnym. Jeśli nie jesteś administratorem globalnym, Twoje konto musi zostać dodane do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwaniem zgodności. Aby usunąć wiadomości, musisz dołączyć do grupy ról Zarządzanie organizacją lub do roli zarządzania wyszukiwaniem i przeczyszczanie. Uprawnienia do tych ról są przypisywane w Centrum [& zgodności.](https://protection.office.com/)

1. [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/microsoft-365/compliance/content-search) aby znaleźć wiadomość do usunięcia.
2. [Połączenie do programu PowerShell & w Centrum zgodności zabezpieczeń.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Jeśli używasz uwierzytelniania wieloskładnikowego, zobacz Połączenie, Microsoft 365 programu PowerShell centrum zabezpieczeń & przy użyciu [uwierzytelniania wieloskładnikowego.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
