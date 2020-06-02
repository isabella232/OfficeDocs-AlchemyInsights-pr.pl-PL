---
title: Odwoływanie lub zastępowanie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509466"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odwoływanie lub zastępowanie wiadomości e-mail w usłudze Microsoft 365

- Można **odwoływać tylko wiadomości, które są wysyłane do osób w organizacji**. Jeśli na przykład wiadomość została wysłana na adres Gmaila, nie możesz jej odwołać.
- Można **odwoływać tylko wiadomości wysłane z programu Outlook 2016 na PC**. Jeśli użytkownik wysyła wiadomość za pomocą programu Outlook dla komputerów Mac lub programu Outlook w sieci Web, nie można jej odwołać.
- Jeśli jesteś administratorem, możesz **odwołać wiadomości w imieniu użytkowników za pomocą programu PowerShell**. Nie można odwołać wiadomości z centrum administracyjnego. Przewiń w dół do "Wyszukaj i usuń wiadomości e-mail w organizacji", aby uzyskać więcej informacji.

**Odwoływanie lub zastępowanie wysłanej wiadomości e-mail**

1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
2. Otwórz wiadomość, którą chcesz przywołać. Aby otworzyć wiadomość, należy kliknąć dwukrotnie. Wybranie wiadomości, która pojawi się w okienku odczytu, nie pozwala na odwołanie wiadomości.
3. Na karcie Wiadomość wybierz pozycję **Akcje**  >  **Przywołuje tę wiadomość**.
4. Wybierz **pozycję Usuń nieprzeczytane kopie tej wiadomości** lub Usuń **nieprzeczytane kopie i zastąp nową wiadomością,** a następnie wybierz przycisk **OK**.
5. Jeśli wysyłasz wiadomość zastępczą, skomponuj ją, a następnie wybierz pozycję **Wyślij**.
6. Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień adresatów w programie Outlook.

Aby uzyskać więcej informacji, w tym jak sprawdzić wycofanie, zobacz [Odwoływanie lub zamienianie wysłanej wiadomości e-mail](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Wyszukiwanie i usuwanie wiadomości e-mail w organizacji*** Aby wyszukiwać i usuwać wiadomości e-mail w organizacji, najłatwiej jest, jeśli jesteś administratorem globalnym. Jeśli nie jesteś administratorem globalnym, Twoje konto musi zostać dodane do grupy ról Menedżera zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwaniem zgodności. Aby usunąć wiadomości, musisz dołączyć do grupy ról Zarządzanie organizacją lub roli zarządzania wyszukiwaniem i przeczyszczaniem. Uprawnienia do tych ról są przypisywane w [Centrum zgodności & zabezpieczeń](https://protection.office.com/).

1. [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/microsoft-365/compliance/content-search) aby znaleźć wiadomość do usunięcia.
2. [Połącz się z centrum zabezpieczeń & compliance center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Jeśli używasz usługi MFA, zobacz [Łączenie się z programem Microsoft 365 security center & Compliance Center PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
