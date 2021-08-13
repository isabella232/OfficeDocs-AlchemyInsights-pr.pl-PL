---
title: 1336 Folder RecoverableItems jest pełny
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061766"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder Elementy do odzyskania jest pełny

W Exchange Online skrzynek pocztowych domyślny limit miejsca do magazynowania dla folderu Elementy do odzyskania wynosi 30 GB. Limit miejsca do magazynowania dla folderu Elementy do odzyskania jest automatycznie zwiększany do 100 GB, jeśli skrzynka pocztowa została umieszczona w związku z postępowaniem sądowym, holdem zbierania elektronicznych materiałów dowodowych lub przypisano do zasad przechowywania.

Po osiągnięciu limitu miejsca do magazynowania w folderze Elementy do odzyskania mają wpływ następujące sposoby na działanie skrzynki pocztowej:

- Użytkownik nie może usuwać elementów ze skrzynki pocztowej.

- Asystent folderów zarządzanych nie może usuwać elementów na podstawie tagu przechowywania ani ustawień folderu zarządzanego.

- W przypadku skrzynek pocztowych, w których włączono odzyskiwanie pojedynczych elementów lub które znajdują się w stanie przechowywania, proces ochrony strony podczas kopiowania w trakcie pisania nie może zachować wersji elementów edytowanych przez użytkownika.

- W przypadku skrzynek pocztowych, w których włączono rejestrowanie inspekcji skrzynki pocztowej, wpisy dziennika inspekcji skrzynek pocztowych nie mogą być zapisywane w podfolderze Inspekcje w folderze Elementy odzyskiwalne.

W przypadku skrzynek pocztowych, które nie są zawieszone, administratorzy mogą użyć polecenia w programie Exchange Online PowerShell, aby usunąć elementy z folderu Elementy `Search-Mailbox -SearchDumpsterOnly -DeleteContent` do odzyskania. Aby uzyskać więcej informacji, zobacz następujące tematy:

- [Wyszukiwanie i usuwanie wiadomości](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

W przypadku skrzynek pocztowych, które znajdują się w stanie przechowywania, administratorzy muszą usunąć to hold, aby można było usuwać elementy z folderu Elementy do odzyskania. Aby uzyskać więcej informacji, zobacz Usuwanie elementów z folderu Elementy [odzyskiwalne w chmurze](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)ze skrzynkami pocztowymi w chmurze.

Aby zapobiec zapełniniu folderu Elementy do odzyskania, administratorzy mogą zwiększyć limit miejsca do magazynowania folderu Elementy do odzyskania dla skrzynek pocztowych w archiwum i skonfigurować zasady przechowywania skrzynki pocztowej, które będą przenosić elementy z folderu Elementy do odzyskania do archiwaowej skrzynki pocztowej użytkownika. Zobacz [Zwiększanie przydziału elementów odzyskiwalnych dla skrzynek pocztowych w hold.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
