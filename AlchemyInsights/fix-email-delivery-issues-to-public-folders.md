---
title: Rozwiąż problemy z dostarczaniem wiadomości e-mail do folderów publicznych z włączoną obsługą poczty e-mail
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910617"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rozwiąż problemy z dostarczaniem wiadomości e-mail do folderów publicznych z włączoną obsługą poczty e-mail

Jeśli nadawców zewnętrznych nie mogą wysyłać wiadomości do folderów publicznych pocztę i nadawców zgłaszany jest błąd: **nie można odnaleźć (550 5.4.1)**, sprawdź domenę poczty e-mail dla folderu publicznego jest skonfigurowana jako domena przekazywania wewnętrznego zamiast autorytatywny domeny:

1. Otwórz [Centrum administracyjnego programu Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Przejdź do **przepływu poczty** \> **akceptowanych domen**, zaznacz zaakceptowana domena, a następnie kliknij przycisk **Edytuj**.

3. W oknie właściwości tego otwierania strony, jeśli ustawiono typ domeny na **autorytatywne**, zmień wartość na **Przekaźnik wewnętrzny** , a następnie kliknij przycisk **Zapisz**.

Jeśli nadawców zewnętrznych wyświetlony błąd, **użytkownik nie ma uprawnień (550 5.7.13)**, uruchom następujące polecenie w [PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , aby zobaczyć jego uprawnienia dla użytkowników anonimowych w folderze publicznym:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na przykład `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Aby umożliwić użytkownikom zewnętrznym na wysłanie wiadomości e-mail do tego folderu publicznego, należy dodać dostęp CreateItems prawo do użytkowników anonimowych. Na przykład `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
