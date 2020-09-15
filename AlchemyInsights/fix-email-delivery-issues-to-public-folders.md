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
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail do folderów publicznych z obsługą poczty

Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty, a nadawcy otrzymają błąd: **nie można znaleźć (550 5.4.1)**, sprawdź, czy domena poczty e-mail folderu publicznego jest skonfigurowana jako wewnętrzna domena przekaźnikowa, a nie domena autorytatywna:

1. Otwórz [Centrum administracyjne programu Exchange (SKK)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Przejdź do obszaru **przepływ poczty** \> , **zaakceptowane**domeny, wybierz zaakceptowaną domenę, a następnie kliknij pozycję **Edytuj**.

3. Na wyświetlonej stronie właściwości, jeśli typ domeny jest ustawiony na wartość **autorytatywna**, Zmień wartość na **przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.

Jeśli nadawcy zewnętrzni otrzymają błąd, **którego nie masz uprawnień (550 5.7.13)**, uruchom następujące polecenie w programie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby wyświetlić uprawnienia dla użytkowników anonimowych w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Aby zezwolić użytkownikom zewnętrznym na wysyłanie wiadomości e-mail do tego folderu publicznego, Dodaj prawo dostępu do elementu o dostępie do użytkownika anonimowego. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
