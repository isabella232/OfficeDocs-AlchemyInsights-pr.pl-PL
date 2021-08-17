---
title: Uprawnienia kalendarza
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046114"
---
# <a name="calendar-permissions"></a>Uprawnienia kalendarza

Użytkownicy mogą zmieniać własne uprawnienia kalendarza Outlook w sieci Web lub innych klientach, ale jako administrator może być konieczne również jego sprawdzenie.  
Polecenie Exchange cmdlet programu PowerShell spowoduje wyświetlanie uprawnień do kalendarza użytkownika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Aby uzyskać więcej informacji, zobacz następujące informacje:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Uprawnienia kalendarza są używane do udostępniania kalendarzy. Aby uzyskać więcej informacji na temat udostępniania kalendarza Outlook kalendarza, zobacz następujące artykuły:

- [Udostępnianie kalendarza programu Outlook innym osobom](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Udostępnianie kalendarza w programie Outlook w sieci Web dla firm](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Aby rozwiązać problemy z uprawnieniem kalendarza, możesz [użyć Asystent odzyskiwania i pomocy technicznej](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) kalendarza.