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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013758"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Błędy synchronizacji automatycznej rejestracji urządzeń firmy Apple

"Wykryliśmy, że masz co najmniej jeden token ADE/DEP w stanie błędu. Do czasu rozwiązania stanu błędu dla każdego tokenu, którego dotyczy problem, funkcja ADE nie będzie działać zgodnie z oczekiwaniami".

Ten błąd może wystąpić na kilka sposobów, w tym:

1. Urządzenia mogą nie być synchronizowane z abm/asm do intune
2. Przypisania profilów rejestracji mogą się nie pomylić
3. Urządzenia mogą nie zdać pomyślnie rejestracji ADE

Sprawdź, czy nie wystąpił błąd synchronizacji zgłoszony w konsoli Intune w obszarze Urządzenia > Zarejestruj urządzenia > rejestracja > **tokenów programu rejestracji firmy Apple.**

Jedną z najbardziej typowych przyczyn błędu synchronizacji jest wygaśnięcie bieżącego tokenu. W wielu przypadkach odnowienie tokenu, którego dotyczy problem, rozwiąże ten problem.

Jeśli jeden lub więcej tokenów wygasło, zapoznaj się z następującą dokumentacją, aby w razie potrzeby pomóc w ich odnowieniu:

[Odnawianie tokenu automatycznej rejestracji urządzenia](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ponadto możesz wyświetlić następującą dokumentację, aby zobaczyć potencjalne działania naprawcze dotyczące innych błędów powodujących błędy synchronizacji tokenów:

[Błędy synchronizacji ABM/ASM dotyczące tokenów automatycznej rejestracji urządzenia w systemie iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Błędy synchronizacji ABM/ASM dotyczące tokenów automatycznej rejestracji urządzenia w systemie iOS/iPadOS i macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
