---
title: Ukrywanie folderów publicznych
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315435"
---
# <a name="hide-public-folders"></a>Ukrywanie folderów publicznych

**Aby ukryć całe drzewo folderów publicznych:**

Aby ukryć [całe](https://aka.ms/ControlPF) drzewo folderów publicznych przed selektywnym lub wszystkim użytkownikom, skorzystaj z procedury opisanej w tym artykule.

**Aby ukryć określony folder publiczny:**

1. Dodawanie uprawnień dla użytkowników, którzy muszą mieć dostęp do folderu publicznego

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Usuń użytkownika **domyślnego** z **listy** uprawnień:

    `Remove-PublicFolderClientPermission \test1 -User Default`
