---
title: Właściciel nie może utworzyć podfolderu przy użyciu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063134"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Właściciel nie może utworzyć podfolderu przy użyciu Outlook

**Obecnie występuje problem z utworzeniem podfolderów przez właścicieli folderów publicznych przy użyciu Outlook. Ten problem zostanie wkrótce rozwiązany.**

W międzyczasie możesz skorzystać z jednego z następujących obejść:

1. Utwórz Outlook dla komputerów Mac, ponieważ problem dotyczy tylko okna Outlook dla komputerów stacjonarnych (wszystkie wersje)
2. Zleć administratorowi utworzenie podfolderu przy użyciu powłoki EXO lub Centrum administracyjnego programu SharePoint
3. Zmienianie folderu DefaultPublicFolderMailbox/EffectivePublicFolderMailbox w użytkowniku na inną skrzynkę pocztową niż skrzynka pocztowa zawartości folderu powodującego problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odczekaj godzinę, uruchom ponownie klienta programu Outlook