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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819918"
---
# <a name="calendar-permissions"></a>Uprawnienia kalendarza

Użytkownicy mogą zmieniać własne uprawnienia kalendarza w aplikacji Outlook w sieci Web lub innych klientach, ale jako administrator może być konieczne również jego sprawdzenie.  
Polecenie cmdlet programu PowerShell dla programu Exchange umożliwia wyświetlanie uprawnień w kalendarzu użytkownika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Aby uzyskać więcej informacji, zobacz następujące informacje:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Uprawnienia kalendarza są używane do udostępniania kalendarzy. Aby uzyskać więcej informacji na temat udostępniania kalendarza programu Outlook, zobacz następujące artykuły:

- [Udostępnianie kalendarza programu Outlook innym osobom](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Udostępnianie kalendarza w aplikacji Outlook w sieci Web dla firm](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Aby rozwiązać problemy z uprawnieniami kalendarza, możesz użyć narzędzia [Asystent odzyskiwania i pomocy](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) technicznej.