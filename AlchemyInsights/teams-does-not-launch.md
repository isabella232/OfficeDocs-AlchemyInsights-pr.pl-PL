---
title: Teams nie uruchamia się
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813354"
---
# <a name="teams-doesnt-launch"></a>Teams nie uruchamia się

Jeśli próbujesz otworzyć program Microsoft Teams ale nie jest on otwierany, spróbuj wykonać następujące czynności:

1. Przejdź do **folderu %appdata%\Microsoft\Teams.**
1. Usuń zawartość folderu.
1. Uruchom ponownie komputer i spróbuj uruchomić Teams.

Może być konieczne ponowne zainstalowanie Teams. Aby ponownie zainstalować:

1. Odinstaluj Teams przy użyciu Panelu sterowania.
1. Przejdź do **folderu %appdata%\Microsoft\Teams\Application Cache.**
1. Usuń zawartość folderu.
1. Przejdź do **folderu %appdata%\Microsoft\teams\Cache.**
1. Usuń zawartość folderu.
1. Uruchom ponownie komputer, a następnie pobierz i zainstaluj Teams.

Jeśli chcesz uruchomić w swojej dzierżawie diagnostykę dla określonego użytkownika, który nie może się zalogować, rozpocznij nowe wyszukiwanie, słowa kluczowego **TeamsUserUnableToSignIn** i postępuj zgodnie z monitami.