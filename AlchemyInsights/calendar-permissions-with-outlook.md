---
title: Uprawnienia kalendarza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862172"
---
# <a name="calendar-permissions"></a>Uprawnienia kalendarza

Użytkownicy mogą zmieniać własne uprawnienia kalendarza za pomocą aplikacji Outlook w sieci Web lub innych klientach, ale jako administrator może być również konieczne zbadanie.  
W ydlet cmdlet programu Exchange PowerShell wyświetli uprawnienia do kalendarza użytkownika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Aby uzyskać więcej informacji, zobacz następujące informacje:

- [Get-MailBoxFolderPermission (Niesie zechcenie skrzynki pocztowej)](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission Set-MailBoxPermission Set-MailBox](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailBoxFolderPermission (Dodawanie skrzynki pocztowej)](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Uprawnienia kalendarza są używane w udostępnianiu kalendarzy, aby wyświetlić więcej informacji na temat udostępniania kalendarza programu Outlook, zobacz następujące artykuły:

- [Udostępnianie kalendarza programu Outlook innym osobom](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Udostępnianie kalendarza w aplikacji Outlook dla firm w sieci Web](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Aby rozwiązać problem z uprawnieniem kalendarza, można użyć narzędzia [Pomoc techniczna i Asystent odzyskiwania.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)