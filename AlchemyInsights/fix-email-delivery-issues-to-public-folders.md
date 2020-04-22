---
title: Rozwiązywanie problemów z dostarczaniem wiadomości e-mail do folderów publicznych z obsługą poczty
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716362"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="932ed-102">Rozwiązywanie problemów z dostarczaniem wiadomości e-mail do folderów publicznych z obsługą poczty</span><span class="sxs-lookup"><span data-stu-id="932ed-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="932ed-103">Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty, a nadawcy otrzymają błąd: **nie można odnaleźć (550 5.4.1),** sprawdź, czy domena poczty e-mail dla folderu publicznego jest skonfigurowana jako wewnętrzna domena przekazywania zamiast autorytatywnej domeny:</span><span class="sxs-lookup"><span data-stu-id="932ed-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="932ed-104">Otwórz [centrum administracyjne programu Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="932ed-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="932ed-105">Przejdź do usługi **Domena zaakceptowana** **przepływ** \> poczty , wybierz zaakceptowana domena, a następnie kliknij przycisk **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="932ed-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="932ed-106">Na otwartej stronie właściwości, jeśli typ domeny jest ustawiony na **Autorytatywny,** zmień wartość na **Przekaźnik wewnętrzny,** a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="932ed-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="932ed-107">Jeśli nadawcy zewnętrzni otrzymają **błąd, który nie ma uprawnień (550 5.7.13),** uruchom następujące polecenie w [programie Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aby wyświetlić uprawnienia dla anonimowych użytkowników w folderze publicznym:</span><span class="sxs-lookup"><span data-stu-id="932ed-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="932ed-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="932ed-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="932ed-109">Aby umożliwić użytkownikom zewnętrznym wysyłanie wiadomości e-mail do tego folderu publicznego, należy dodać prawo dostępu CreateItems do użytkownika Anonimowy.</span><span class="sxs-lookup"><span data-stu-id="932ed-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="932ed-110">Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="932ed-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
