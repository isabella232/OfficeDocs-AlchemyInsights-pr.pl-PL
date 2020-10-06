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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366474"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail do folderów publicznych z obsługą poczty

Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty, a nadawcy otrzymają błąd: **nie można znaleźć (550 5.4.1)**, sprawdź, czy domena poczty e-mail folderu publicznego jest skonfigurowana jako wewnętrzna domena przekaźnikowa, a nie domena autorytatywna:

1. Otwórz [Centrum administracyjne programu Exchange (SKK)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Przejdź do obszaru **przepływ poczty** \> , **zaakceptowane**domeny, wybierz zaakceptowaną domenę, a następnie kliknij pozycję **Edytuj**.

3. Na wyświetlonej stronie właściwości, jeśli typ domeny jest ustawiony na wartość **autorytatywna**, Zmień wartość na **przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.

Jeśli nadawcy zewnętrzni otrzymają błąd, **którego nie masz uprawnień (550 5.7.13)**, uruchom następujące polecenie w programie [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby wyświetlić uprawnienia dla użytkowników anonimowych w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Aby zezwolić użytkownikom zewnętrznym na wysyłanie wiadomości e-mail do tego folderu publicznego, Dodaj prawo dostępu do elementu o dostępie do użytkownika anonimowego. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
