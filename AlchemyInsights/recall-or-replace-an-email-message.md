---
title: Odwoływanie lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 461969bee3b871fd2c4a8418406ea2b6de791191
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770818"
---
# <a name="recall-or-replace-an-email-message"></a>Odwoływanie lub zamienianie wiadomości e-mail

- Możesz **tylko odwoływania wiadomości, które są wysyłane do osoby w organizacji**. Jeśli wiadomość została wysłana na adres Gmail, na przykład, nie można wywołać ją.
- Możesz **tylko odwoływania wiadomości wysłane z Outlook 2016 dla komputerów PC**. Jeśli użytkownik wysyła wiadomości za pomocą programu Outlook w sieci web lub programu Outlook dla komputerów Macintosh, nie może je wycofać.
- Jeśli jesteś administratorem, możesz **odwoływania wiadomości w imieniu użytkowników przy użyciu środowiska PowerShell**. Nie można odwołać wiadomości z Centrum administracyjnego. Przewiń w dół do "Wyszukiwanie i usuwanie wiadomości e-mail w firmie" Aby uzyskać więcej informacji.

***Odwoływanie lub zamienianie wiadomości e-mail wysłanej przez Ciebie***
1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
2. Otwórz wiadomość, która ma zostać odwołana. Należy kliknąć dwukrotnie Otwórz wiadomość. Zaznaczając wiadomość — będą wyświetlane w okienku odczytu nie pozwoli odwołać wiadomość.
3. Na karcie wiadomość zaznacz **Akcje** > **Odwołaj tę wiadomość**.
4. **Usunąć nieprzeczytane kopie tej wiadomości** lub **usunąć nieprzeczytane kopie i zastąpić je nową wiadomością**, a następnie wybierz **OK**.
5. Jeśli wysyłasz wiadomość wymiana redagowania wiadomości, a następnie zaznacz pole wyboru **Wyślij**.
6. Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień adresatów w programie Outlook. 

Aby uzyskać więcej informacji, w tym jak sprawdzić na przypomnienie zobacz [odwołanie lub zamień wysłaną wiadomość e-mail](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Wyszukiwanie i usuwanie wiadomości e-mail w organizacji*** Do wyszukiwania i usuwania wiadomości w organizacji, najłatwiej jest w przypadku globalnego administratora. Jeśli nie jesteś administratorem globalnym, należy dodać konta do grupy roli Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania wyszukiwania zgodności. Aby usunąć wiadomości, będziesz musiał przyłączyć się do grupy ról Zarządzanie organizacją lub Rola zarządzania wyszukiwania i czyszczenie. Uprawnienia do tych ról są przypisywane w [Centrum zgodności zabezpieczeń &](https://protection.office.com/).

1. [Tworzenie zawartości wyszukiwania](https://docs.microsoft.com/office365/securitycompliance/content-search) , aby odnaleźć wiadomości do usunięcia.
2. [Podłącz do środowiska PowerShell Centrum zgodności & zabezpieczeń](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Jeśli używasz MFA, zobacz [Nawiązywanie połączenia z & zabezpieczeń usługi Office 365 PowerShell Centrum zgodności za pomocą wieloczynnikowe uwierzytelnianie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 