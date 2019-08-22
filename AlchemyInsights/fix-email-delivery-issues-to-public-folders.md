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
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525132"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiąż problemy z dostarczaniem wiadomości e-mail do folderów publicznych z włączoną obsługą poczty e-mail

Jeśli nadawców zewnętrznych nie mogą wysyłać wiadomości do folderów publicznych pocztę i nadawców zgłaszany jest błąd: **nie można odnaleźć (550 5.4.1)**, sprawdź domenę poczty e-mail dla folderu publicznego jest skonfigurowana jako domena przekazywania wewnętrznego zamiast autorytatywny domeny:

1. Otwórz [Centrum administracyjnego programu Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Przejdź do **przepływu poczty** \> **akceptowanych domen**, zaznacz zaakceptowana domena, a następnie kliknij przycisk **Edytuj**.

3. W oknie właściwości tego otwierania strony, jeśli ustawiono typ domeny na **autorytatywne**, zmień wartość na **Przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.

Jeśli nadawców zewnętrznych wyświetlony błąd, **użytkownik nie ma uprawnień (550 5.7.13)**, uruchom następujące polecenie w [PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby zobaczyć jego uprawnienia dla użytkowników anonimowych w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Aby umożliwić użytkownikom zewnętrznym na wysłanie wiadomości e-mail do tego folderu publicznego, należy dodać dostęp CreateItems prawo do użytkowników anonimowych. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
