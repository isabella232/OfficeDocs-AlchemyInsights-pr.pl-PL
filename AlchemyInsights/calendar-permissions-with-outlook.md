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
# <a name="calendar-permissions"></a><span data-ttu-id="931e9-102">Uprawnienia kalendarza</span><span class="sxs-lookup"><span data-stu-id="931e9-102">Calendar Permissions</span></span>

<span data-ttu-id="931e9-103">Użytkownicy mogą zmieniać własne uprawnienia kalendarza za pomocą aplikacji Outlook w sieci Web lub innych klientach, ale jako administrator może być również konieczne zbadanie.</span><span class="sxs-lookup"><span data-stu-id="931e9-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="931e9-104">W ydlet cmdlet programu Exchange PowerShell wyświetli uprawnienia do kalendarza użytkownika:</span><span class="sxs-lookup"><span data-stu-id="931e9-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="931e9-105">Aby uzyskać więcej informacji, zobacz następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="931e9-105">To see more information see the following:</span></span>

- [<span data-ttu-id="931e9-106">Get-MailBoxFolderPermission (Niesie zechcenie skrzynki pocztowej)</span><span class="sxs-lookup"><span data-stu-id="931e9-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="931e9-107">Set-MailboxFolderPermission Set-MailBoxPermission Set-MailBox</span><span class="sxs-lookup"><span data-stu-id="931e9-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="931e9-108">Add-MailBoxFolderPermission (Dodawanie skrzynki pocztowej)</span><span class="sxs-lookup"><span data-stu-id="931e9-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="931e9-109">Uprawnienia kalendarza są używane w udostępnianiu kalendarzy, aby wyświetlić więcej informacji na temat udostępniania kalendarza programu Outlook, zobacz następujące artykuły:</span><span class="sxs-lookup"><span data-stu-id="931e9-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="931e9-110">Udostępnianie kalendarza programu Outlook innym osobom</span><span class="sxs-lookup"><span data-stu-id="931e9-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="931e9-111">Udostępnianie kalendarza w aplikacji Outlook dla firm w sieci Web</span><span class="sxs-lookup"><span data-stu-id="931e9-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="931e9-112">Aby rozwiązać problem z uprawnieniem kalendarza, można użyć narzędzia [Pomoc techniczna i Asystent odzyskiwania.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="931e9-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>