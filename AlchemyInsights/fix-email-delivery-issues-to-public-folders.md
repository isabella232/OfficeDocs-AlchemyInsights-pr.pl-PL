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
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiązywanie problemów z dostarczaniem wiadomości e-mail do folderów publicznych z obsługą poczty

Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty, a nadawcy otrzymają błąd: **nie można odnaleźć (550 5.4.1),** sprawdź, czy domena poczty e-mail dla folderu publicznego jest skonfigurowana jako wewnętrzna domena przekazywania zamiast autorytatywnej domeny:

1. Otwórz [centrum administracyjne programu Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Przejdź do usługi **Domena zaakceptowana** **przepływ** \> poczty , wybierz zaakceptowana domena, a następnie kliknij przycisk **Edytuj**.

3. Na otwartej stronie właściwości, jeśli typ domeny jest ustawiony na **Autorytatywny,** zmień wartość na **Przekaźnik wewnętrzny,** a następnie kliknij przycisk **Zapisz**.

Jeśli nadawcy zewnętrzni otrzymają **błąd, który nie ma uprawnień (550 5.7.13),** uruchom następujące polecenie w [programie Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aby wyświetlić uprawnienia dla anonimowych użytkowników w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Aby umożliwić użytkownikom zewnętrznym wysyłanie wiadomości e-mail do tego folderu publicznego, należy dodać prawo dostępu CreateItems do użytkownika Anonimowy. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
