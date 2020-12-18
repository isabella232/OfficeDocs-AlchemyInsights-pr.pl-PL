---
title: Błędy synchronizacji automatycznego rejestrowania urządzeń firmy Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714828"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Błędy synchronizacji automatycznego rejestrowania urządzeń firmy Apple

"Wykryto, że masz co najmniej jeden token ADE/DEP w stanie błędu. Do momentu rozwiązania błędu w odniesieniu do każdego z tokenów, których dotyczy problem, funkcja ADE nie będzie działać w przypadku tego samego ".

Ten błąd może być manifestem na kilka sposobów, takich jak:

1. Urządzenia mogą nie być synchronizowane z ABM/ASM do usługi Intune
2. Zadania profilu rejestracji mogą być błędne
3. Urządzenia mogą nie zakończyć się pomyślnie rejestracji w programie ADE

Sprawdź, czy w konsoli usługi Intune Wystąpił błąd synchronizacji w obszarze **urządzenia > zarejestrować urządzenia > rejestracji firmy Apple > tokeny programu rejestracji** i zapoznaj się z poniższą dokumentacją w celu wyświetlenia ewentualnych środków zaradczych:

[Błędy synchronizacji ABM/ASM dla tokenów automatycznego rejestrowania urządzeń z systemami iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
