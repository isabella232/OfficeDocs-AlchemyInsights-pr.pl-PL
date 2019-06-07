---
title: Rozwiąż problemy z dostarczaniem wiadomości e-mail do folderów publicznych z włączoną obsługą poczty e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752681"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="55c79-102">Rozwiąż problemy z dostarczaniem wiadomości e-mail do folderów publicznych z włączoną obsługą poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="55c79-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="55c79-103">Jeśli nadawców zewnętrznych nie mogą wysyłać wiadomości do folderów publicznych pocztę i nadawców zgłaszany jest błąd: **nie można odnaleźć (550 5.4.1)**, sprawdź domenę poczty e-mail dla folderu publicznego jest skonfigurowana jako domena przekazywania wewnętrznego zamiast autorytatywny domeny:</span><span class="sxs-lookup"><span data-stu-id="55c79-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="55c79-104">Otwórz [Centrum administracyjnego programu Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="55c79-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="55c79-105">Przejdź do **przepływu poczty** \> **akceptowanych domen**, zaznacz zaakceptowana domena, a następnie kliknij przycisk **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="55c79-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="55c79-106">W oknie właściwości tego otwierania strony, jeśli ustawiono typ domeny na **autorytatywne**, zmień wartość na **Przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="55c79-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="55c79-107">Jeśli nadawców zewnętrznych wyświetlony błąd, **użytkownik nie ma uprawnień (550 5.7.13)**, uruchom następujące polecenie w [PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby zobaczyć jego uprawnienia dla użytkowników anonimowych w folderze publicznym:</span><span class="sxs-lookup"><span data-stu-id="55c79-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="55c79-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="55c79-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="55c79-109">Aby umożliwić użytkownikom zewnętrznym na wysłanie wiadomości e-mail do tego folderu publicznego, należy dodać dostęp CreateItems prawo do użytkowników anonimowych.</span><span class="sxs-lookup"><span data-stu-id="55c79-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="55c79-110">Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="55c79-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
