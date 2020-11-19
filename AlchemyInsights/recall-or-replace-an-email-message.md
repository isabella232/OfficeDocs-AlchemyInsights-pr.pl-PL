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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353516"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odwoływanie lub zamienianie wiadomości e-mail w programie Microsoft 365

- Możesz **odwołać tylko wiadomości wysłane do osób w organizacji**. Jeśli na przykład wiadomość została wysłana na adres Gmail, nie można jej odwołać.
- Możesz **odwołać tylko wiadomości wysyłane z programu Outlook dla komputerów PC**. Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Mac lub aplikacji Outlook w sieci Web, nie można jej odwołać.
- Jako Administrator dzierżawy możesz **odwołać wiadomości w imieniu użytkowników za pomocą programu PowerShell** (Aby uzyskać więcej informacji, zobacz: [Wyszukiwanie i usuwanie wiadomości e-mail](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Nie można odwołać wiadomości z centrum administracyjnego. Aby uzyskać więcej informacji, przewiń w dół do listy "wyszukiwanie i usuwanie wiadomości e-mail w organizacji".

**Odwoływanie lub zamienianie wysłanej wiadomości e-mail**

1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
2. Otwórz wiadomość, którą chcesz odwołać. Musisz kliknąć dwukrotnie, aby otworzyć wiadomość. Wybranie wiadomości w celu wyświetlenia jej w okienku odczytu nie pozwala na odwołanie wiadomości.
3. Na karcie wiadomość wybierz pozycję **Akcje**  >  **odwołaj tę wiadomość**.
4. Wybierz pozycję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i zastąp je nową wiadomością**, a następnie wybierz **przycisk OK**.
5. Jeśli wysyłasz wiadomość zastępującą, Zredaguj wiadomość, a następnie wybierz pozycję **Wyślij**.
6. Sukces lub niepowodzenie odwołania wiadomości zależy od ustawień adresatów w programie Outlook.

Aby uzyskać więcej informacji, w tym sposób sprawdzania odwołania, zobacz [odwoływanie lub zamienianie wysłanej wiadomości e-mail](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Wyszukiwanie i usuwanie wiadomości e-mail w organizacji_** jest najłatwiej, jeśli jesteś administratorem globalnym. Jeśli nie jesteś administratorem globalnym, konto należy dodać do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwaniem zgodności. Aby usunąć wiadomości, musisz przyłączyć się do grupy ról zarządzania organizacją lub wyszukiwania i usuwania. Uprawnienia do tych ról są przypisywane w [Centrum zabezpieczeń & zgodności](https://protection.office.com/).

1. [Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/microsoft-365/compliance/content-search) , aby znaleźć wiadomość, którą chcesz usunąć.
2. [Nawiązywanie połączenia z programem PowerShell w centrum zgodności & zabezpieczeniami](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Jeśli korzystasz z uwierzytelniania wieloskładnikowe (Multi-Factor Authentication), zobacz [nawiązywanie połączenia z programem Microsoft 365 Security & Centrum zgodności programu PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
