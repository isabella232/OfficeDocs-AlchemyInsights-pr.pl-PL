---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749140"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook

**Istnieje stały problem z właścicielami folderów publicznych tworzenia podfolderów za pomocą programu Outlook. Problem zostanie wkrótce rozwiązany.**

W międzyczasie należy użyć jednego z następujących rozwiązań:

1. Tworzenie podfolderu za pomocą programu Outlook dla komputerów MAC w celu utworzenia podfolderu, ponieważ problem dotyczy tylko systemu Outlook dla komputerów stacjonarnych (wszystkie wersje)
2. Czy administrator utworzyć podfolder przy użyciu EXO Shell lub EAC
3. Zmień domyślną skrzynkę adresową folderu  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odczekanie godziny, ponowne uruchomienie klienta programu Outlook