---
title: 1336 Folder RecoverableItems jest pełny
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720262"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folder Elementy do odzyskania jest pełny

W przypadku skrzynek pocztowych usługi Exchange Online domyślny limit miejsca dla folderu Elementy możliwe do odzyskania wynosi 30 GB. Limit magazynowania folderu Elementy możliwe do odzyskania jest automatycznie zwiększany do 100 GB, jeśli skrzynka pocztowa zostanie umieszczona w wstrzymaniu postępowania sądowego, blokadzie zbierania elektronicznych materiałów dowodowych lub jest przypisana do zasad przechowywania.

Gdy folder Elementy możliwe do odzyskania osiągnie limit magazynowania, działanie skrzynki pocztowej jest zagrożone w następujący sposób:

- Użytkownik nie może usuwać elementów ze skrzynki pocztowej.

- Asystent folderów zarządzanych nie może usuwać elementów na podstawie tagu przechowywania lub ustawień folderu zarządzanego.

- W przypadku skrzynek pocztowych, w których włączona lub wstrzymana jest funkcja odzyskiwania pojedynczego elementu, proces ochrony strony kopiowania przy zapisie nie może obsługiwać wersji elementów edytowanych przez użytkownika.

- W przypadku skrzynek pocztowych z włączonym rejestrowaniem inspekcji skrzynek pocztowych w podfolderze Inspekcje w folderze Elementy podlegające odzyskiwalnej nie można zapisywać żadnych wpisów dziennika inspekcji skrzynki pocztowej.

W przypadku skrzynek pocztowych, które nie są `Search-Mailbox -SearchDumpsterOnly -DeleteContent` wstrzymane, administratorzy mogą użyć polecenia programu Exchange Online PowerShell do usuwania elementów w folderze Elementy do odzyskania. Aby uzyskać więcej informacji, zobacz następujące tematy:

- [Wyszukiwanie i usuwanie wiadomości](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Szukaj-Skrzynka pocztowa](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

W przypadku wstrzymanych skrzynek pocztowych administratorzy muszą usunąć blokadę, zanim będą mogli usunąć elementy z folderu Elementy do odzyskania. Aby uzyskać więcej informacji, zobacz [Usuwanie elementów w folderze Elementy możliwe do odzyskania w chmurowych skrzynkach pocztowych wstrzymanych](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Aby zapobiec zapełnieniu folderu Elementy do odzyskania, administratorzy mogą zwiększyć limit magazynowania folderu Elementy odzyskiwalne dla wstrzymanych skrzynek pocztowych i skonfigurować zasady przechowywania skrzynek pocztowych, które przenoszą elementy z folderu Elementy do odzyskania do archiwalnej skrzynki pocztowej użytkownika. Zobacz [Zwiększanie przydziału elementów do odzyskania dla wstrzymanych skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
