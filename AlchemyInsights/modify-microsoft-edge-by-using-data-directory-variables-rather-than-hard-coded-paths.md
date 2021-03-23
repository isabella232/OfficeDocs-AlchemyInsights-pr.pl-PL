---
title: Modyfikowanie programu Microsoft Edge przy użyciu zmiennych katalogu danych zamiast ścieżek kodowych
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035824"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modyfikowanie programu Microsoft Edge przy użyciu zmiennych katalogu danych zamiast ścieżek kodowych

Aby na przykład w systemie Windows przechowywać dane profilu w danych aplikacji lokalnej użytkownika, a nie w lokalizacji domyślnej, ustaw zasady *UserDataDir* na **wartość ${local_app_data}\Edge\Profile.**

Aby uzyskać więcej informacji, zobacz Tworzenie zmiennych katalogu danych użytkownika programu [Microsoft Edge.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)