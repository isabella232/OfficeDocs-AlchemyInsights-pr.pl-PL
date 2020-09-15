---
title: Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail do folderów publicznych z obsługą poczty
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677938"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="753d2-102">Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail do folderów publicznych z obsługą poczty</span><span class="sxs-lookup"><span data-stu-id="753d2-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="753d2-103">Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty, a nadawcy otrzymają błąd: **nie można znaleźć (550 5.4.1)**, sprawdź, czy domena poczty e-mail folderu publicznego jest skonfigurowana jako wewnętrzna domena przekaźnikowa, a nie domena autorytatywna:</span><span class="sxs-lookup"><span data-stu-id="753d2-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="753d2-104">Otwórz [Centrum administracyjne programu Exchange (SKK)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="753d2-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="753d2-105">Przejdź do obszaru **przepływ poczty** \> , **zaakceptowane**domeny, wybierz zaakceptowaną domenę, a następnie kliknij pozycję **Edytuj**.</span><span class="sxs-lookup"><span data-stu-id="753d2-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="753d2-106">Na wyświetlonej stronie właściwości, jeśli typ domeny jest ustawiony na wartość **autorytatywna**, Zmień wartość na **przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="753d2-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="753d2-107">Jeśli nadawcy zewnętrzni otrzymają błąd, **którego nie masz uprawnień (550 5.7.13)**, uruchom następujące polecenie w programie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby wyświetlić uprawnienia dla użytkowników anonimowych w folderze publicznym:</span><span class="sxs-lookup"><span data-stu-id="753d2-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="753d2-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="753d2-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="753d2-109">Aby zezwolić użytkownikom zewnętrznym na wysyłanie wiadomości e-mail do tego folderu publicznego, Dodaj prawo dostępu do elementu o dostępie do użytkownika anonimowego.</span><span class="sxs-lookup"><span data-stu-id="753d2-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="753d2-110">Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="753d2-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
