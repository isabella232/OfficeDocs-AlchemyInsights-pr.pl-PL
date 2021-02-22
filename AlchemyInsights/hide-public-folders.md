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
# <a name="hide-public-folders"></a><span data-ttu-id="46405-102">Ukrywanie folderów publicznych</span><span class="sxs-lookup"><span data-stu-id="46405-102">Hide public folders</span></span>

<span data-ttu-id="46405-103">**Aby ukryć całe drzewo folderów publicznych:**</span><span class="sxs-lookup"><span data-stu-id="46405-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="46405-104">Aby ukryć [całe](https://aka.ms/ControlPF) drzewo folderów publicznych przed selektywnym lub wszystkim użytkownikom, skorzystaj z procedury opisanej w tym artykule.</span><span class="sxs-lookup"><span data-stu-id="46405-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="46405-105">**Aby ukryć określony folder publiczny:**</span><span class="sxs-lookup"><span data-stu-id="46405-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="46405-106">Dodawanie uprawnień dla użytkowników, którzy muszą mieć dostęp do folderu publicznego</span><span class="sxs-lookup"><span data-stu-id="46405-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="46405-107">Usuń użytkownika **domyślnego** z **listy** uprawnień:</span><span class="sxs-lookup"><span data-stu-id="46405-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
