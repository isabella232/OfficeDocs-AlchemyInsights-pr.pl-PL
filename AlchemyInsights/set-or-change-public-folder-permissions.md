---
title: Ustawianie lub Zmienianie uprawnień do folderów publicznych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734679"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="e1f39-102">Uprawnienia i foldery publiczne</span><span class="sxs-lookup"><span data-stu-id="e1f39-102">Permissions and Public Folders</span></span>

<span data-ttu-id="e1f39-103">Uprawnienia do folderów publicznych można zmienić za pomocą programu Outlook, centrum administracyjnego programu Exchange (EAC) lub programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e1f39-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="e1f39-104">Aby uzyskać instrukcje programu Outlook, [kliknij tutaj](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="e1f39-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="e1f39-105">Dla EAC, zapoznaj się z [tym artykułem](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) , aby uzyskać instrukcje.</span><span class="sxs-lookup"><span data-stu-id="e1f39-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="e1f39-106">Dla programu PowerShell, odnoszą się do [tego artykułu](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) , aby uzyskać instrukcje dotyczące korzystania z apletu Dodaj PublicFolderClientPermission.</span><span class="sxs-lookup"><span data-stu-id="e1f39-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="e1f39-107">Jeśli potrzebujesz instrukcji nawiązywania połączenia z programem Exchange PowerShell, kliknij [tutaj](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="e1f39-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="e1f39-108">Jeśli **użytkownicy zewnętrzni nie mogą wysyłać wiadomości e-mail do folderu publicznego z włączoną obsługą poczty**e-mail, powodem może być brak uprawnień wymaganych do dostarczania zewnętrznej poczty elektronicznej w folderze publicznym.</span><span class="sxs-lookup"><span data-stu-id="e1f39-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="e1f39-109">Można to naprawić za pomocą instrukcji programu Outlook w tym [miejscu](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)lub instrukcje programu PowerShell [tutaj](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="e1f39-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

