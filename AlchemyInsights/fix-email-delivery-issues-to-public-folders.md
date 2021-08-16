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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068822"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail do folderów publicznych z obsługą poczty

Jeśli nadawcy zewnętrzni nie mogą wysyłać wiadomości do folderów publicznych z włączoną obsługą poczty i nadawcy otrzymają komunikat o błędzie: nie można odnaleźć **(550 5.4.1),** sprawdź, czy domena poczty e-mail folderu publicznego jest skonfigurowana jako domena przekazywania wewnętrznego zamiast domeny autorytatywnej:

1. Otwórz [centrum Exchange administracyjnego .](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Przejdź do **przepływu poczty** \> **zaakceptowane domeny,** zaznacz zaakceptowaną domenę, a następnie kliknij pozycję **Edytuj**.

3. Jeśli na stronie właściwości ustawiono typ domeny Autorytatywny, zmień wartość na Przekazywanie wewnętrzne, a **następnie** kliknij przycisk **Zapisz.**

Jeśli nadawcy zewnętrzni otrzymają błąd, że nie masz uprawnień **(550 5.7.13),** uruchom następujące polecenie w programie [Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aby wyświetlić uprawnienia użytkowników anonimowych w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Aby umożliwić użytkownikom zewnętrznym wysyłanie wiadomości e-mail do tego folderu publicznego, dodaj dostęp CreateItems bezpośrednio do użytkownika anonimowego. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
