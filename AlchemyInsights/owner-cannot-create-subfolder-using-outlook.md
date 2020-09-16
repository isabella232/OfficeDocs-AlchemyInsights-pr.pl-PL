---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665728"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook

**W przypadku tworzenia podfolderów za pomocą programu Outlook jest już dostępny problem z właścicielami folderów publicznych. Problem zostanie wkrótce rozwiązany.**

W międzyczasie Użyj jednego z poniższych obejść:

1. Tworzenie podfolderu przy użyciu programu Outlook dla komputerów MAC w celu uzyskania wpływu tylko na program Outlook dla komputerów stacjonarnych (wszystkie wersje)
2. Tworzenie podfolderu przez administratora za pomocą powłoki EXO lub narzędzia SKK
3. Zmienianie DefaultPublicFolderMailbox/EffectivePublicFolderMailbox użytkownika na inną skrzynkę pocztową niż Skrzynka pocztowa zawartości folderu powodującego problem  
    - *Set-Mailbox Użytkownik1 DefaultPublicFolderMailbox PubMBX3*
4. Poczekaj na godzinę, ponownie uruchom klienta programu Outlook