---
title: Błędy synchronizacji automatycznej rejestracji urządzeń firmy Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448932"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Błędy synchronizacji automatycznej rejestracji urządzeń firmy Apple

"Wykryliśmy, że masz co najmniej jeden token ADE/DEP, które znajdują się w stanie błędu. Do czasu rozwiązania stanu błędu dla każdego tokenu, którego dotyczy problem, funkcja ADE nie będzie działać zgodnie z oczekiwaniami".

Ten błąd może wystąpić na wiele sposobów, takich jak:

1. Urządzenia mogą nie być synchronizowane z abm/asm w usłudze Intune
2. Przypisania profilów rejestracji mogą się nie pomylić
3. Urządzenia mogą nie ukończyć pomyślnie rejestracji ADE

Sprawdź, czy nie wystąpił błąd synchronizacji zgłoszony w konsoli Intune w obszarze Urządzenia > Zarejestruj urządzenia > rejestracji firmy Apple > **tokenów programu rejestracji.**

Jedną z najbardziej typowych przyczyn błędu synchronizacji jest wygaśnięcie bieżącego tokenu. W wielu przypadkach odnowienie tokenu, którego dotyczy problem, rozwiąże ten problem.

Jeśli co najmniej jeden z Twoich tokenów wygasł, zapoznaj się z następującą dokumentacją, aby ułatwić odnawianie ich w razie potrzeby:

[Odnawianie tokenu automatycznej rejestracji urządzenia](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ponadto możesz zobaczyć następującą dokumentację, aby zobaczyć potencjalne działania naprawcze dotyczące innych błędów powodujących błędy synchronizacji tokenów:

[Błędy synchronizacji ABM/ASM dla tokenów automatycznej rejestracji urządzeń dla systemów iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Błędy synchronizacji ABM/ASM dla tokenów automatycznej rejestracji urządzeń dla systemów iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
