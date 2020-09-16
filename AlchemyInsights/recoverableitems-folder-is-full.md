---
title: 1336 RecoverableItems folder jest pełny
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741277"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder Elementy odzyskiwalne jest pełny

W przypadku skrzynek pocztowych usługi Exchange Online domyślny limit przestrzeni dyskowej dla folderu Elementy odzyskiwalne wynosi 30 GB. Limit magazynowania folderu Elementy odzyskiwalne jest automatycznie zwiększany do 100 GB, jeśli skrzynka pocztowa jest umieszczona w ramach wstrzymania, wstrzymania zbierania elektronicznych materiałów dowodowych lub przypisana do zasad przechowywania.

Jeśli folder Elementy odzyskiwalne osiągnie limit miejsca na przechowywanie, funkcje skrzynek pocztowych będą miały wpływ na następujące sposoby:

- Użytkownik nie może usuwać elementów ze skrzynki pocztowej.

- Asystent folderów zarządzanych nie może usuwać elementów na podstawie tagu przechowywania lub ustawień folderu zarządzanego.

- W przypadku skrzynek pocztowych, w których włączono funkcję odzyskiwania pojedynczego elementu lub są one zablokowane, proces ochrony przed zapisem na stronie kopiowania nie obsługuje wersji elementów edytowanych przez użytkownika.

- W przypadku skrzynek pocztowych z włączonym rejestrowaniem inspekcji skrzynek pocztowych nie można zapisywać wpisów dziennika inspekcji skrzynki pocztowej w podfolderze inspekcje w folderze Elementy do odzyskania.

W przypadku skrzynek pocztowych, które nie są przechowywane, Administratorzy mogą użyć tego `Search-Mailbox -SearchDumpsterOnly -DeleteContent` polecenia w programie Exchange Online PowerShell, aby usunąć elementy z folderu Elementy odzyskiwalne. Aby uzyskać więcej informacji, zobacz następujące tematy:

- [Wyszukiwanie i usuwanie wiadomości](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Wyszukiwanie — Skrzynka pocztowa](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

W przypadku skrzynek pocztowych zablokowanych Administratorzy muszą usunąć blokadę, zanim będą mogli usunąć elementy z folderu Elementy odzyskiwalne. Aby uzyskać więcej informacji, zobacz [usuwanie elementów w folderze Elementy odzyskiwalne w skrzynkach pocztowych opartych na chmurze](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Aby zapobiec pełnemu zapełnieniu folderu Elementy możliwe, Administratorzy mogą zwiększyć limit magazynowania folderu Elementy odzyskiwalne dla skrzynek pocztowych zablokowanych i skonfigurować zasady przechowywania skrzynek pocztowych, które będą przenosić elementy z folderu Elementy odzyskiwalne do archiwum Skrzynka pocztowa użytkownika. Zobacz [zwiększanie przydziału elementów odzyskiwalnych dla skrzynek pocztowych zablokowanych](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
