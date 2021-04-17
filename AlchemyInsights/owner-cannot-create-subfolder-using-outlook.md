---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836145"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook

**Istnieje bieżący problem z utworzeniem podfolderów przez właścicieli folderów publicznych przy użyciu programu Outlook. Ten problem zostanie wkrótce rozwiązany.**

W międzyczasie możesz skorzystać z jednego z następujących obejść:

1. Utwórz podfolder za pomocą programu Outlook dla komputerów Mac, ponieważ ten problem występuje tylko w programie Outlook dla komputerów stacjonarnych (wszystkie wersje)
2. Zleć administratorowi utworzenie podfolderu przy użyciu powłoki EXO lub Centrum administracyjnego programu SharePoint
3. Zmienianie folderu DefaultPublicFolderMailbox/EffectivePublicFolderMailbox w użytkowniku na inną skrzynkę pocztową niż skrzynka pocztowa zawartości folderu powodującego problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Odczekaj godzinę, uruchom ponownie klienta programu Outlook