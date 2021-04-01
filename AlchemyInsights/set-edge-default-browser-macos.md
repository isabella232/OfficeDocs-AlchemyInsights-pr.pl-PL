---
title: Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu z systemem macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491810"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu z systemem macOS

Użyj jednej z tych dwóch metod, aby ustawić przeglądarkę Microsoft Edge jako domyślną:

Metoda 1. Flashuj urządzenie za pomocą obrazu systemu macOS, w którym program Microsoft Edge został już ustawiony jako domyślna przeglądarka.

Metoda 2. Ustaw zasady DefaultBrowserSettingEnabled, aby monitować użytkownika o ustawienie przeglądarki Microsoft Edge jako domyślnej.

Każda z tych metod umożliwia użytkownikowi zmianę domyślnej przeglądarki. Z tego powodu zalecamy wdrożenie zasad DefaultBrowserSettingEnabled, nawet jeśli została użyta metoda 1. Jeśli po wdrożeniu zasad użytkownik zmieni przeglądarkę domyślną, zasady monituje użytkownika o ustawienie przeglądarki domyślnej z powrotem na Microsoft Edge.
