---
title: 1336 RecoverableItems folder jest pełny
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859006"
---
# <a name="the-recoverable-items-folder-is-full"></a>Przechowalni jest pełny

Dla skrzynek pocztowych Exchange Online w usłudze Office 365 domyślny limit miejsca dla folderu odzyskane elementy wynosi 30 GB. Limit miejsca dla folderu odzyskane elementy automatycznie wzrasta do 100 GB, jeśli Skrzynka pocztowa jest umieszczany na sądowym, przytrzymaj zbierania elektronicznych materiałów dowodowych lub jest przypisana do zasad przechowywania usługi Office 365.

Gdy przechowalni osiągnie limit magazynowania, funkcje skrzynki pocztowej ma wpływ w następujący sposób:

- Użytkownika nie można usunąć elementów ze skrzynki pocztowej.

- Zarządzany Asystent folderów nie można usunąć elementów na podstawie tagu przechowywania lub ustawienia folderów zarządzanych.

- Dla skrzynek pocztowych, które włączonym odzyskiwaniem pojedynczego elementu lub są wstrzymane proces kopiowania przy zapisie strony ochrony nie może utrzymać wersje elementów edytowane przez użytkownika.

- Skrzynki pocztowe, które ma włączone rejestrowanie inspekcji skrzynki pocztowej wpisy dziennika inspekcji skrzynki pocztowej nie można zapisywać w podfolderze audyty w przechowalni.

Skrzynki pocztowe, które nie są zablokowane, Administratorzy można użyć `Search-Mailbox -SearchDumpsterOnly -DeleteContent` polecenia programu PowerShell Online programu Exchange do usuwania elementów w przechowalni. Aby uzyskać więcej informacji, zobacz następujące tematy: 

- [Wyszukiwanie i usuwanie wiadomości](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Skrzynka pocztowa wyszukiwania](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Administratorzy dla skrzynek pocztowych, które zostały wstrzymane, trzeba usunąć ładowni, zanim będą mogli elementy usunięte z folderu elementów do odzyskania. Aby uzyskać więcej informacji zobacz [Usuwanie elementów w przechowalni, przytrzymaj folder chmurowych skrzynek pocztowych na](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Aby zapobiec przechowalni staje się pełne, Administratorzy mogą zwiększyć limit magazynowania odzyskiwalnych elementów folderu dla skrzynek pocztowych na przytrzymaj i ustawianie zasad przechowywania skrzynki pocztowej, która przenosi elementy z folderu odzyskane elementy do archiwum użytkownika Skrzynka pocztowa. Zobacz [zwiększyć odzyskane elementy przydziału dla skrzynek pocztowych na przytrzymaj](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
