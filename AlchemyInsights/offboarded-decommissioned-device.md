---
title: Problemy z usuwaniem wyeksłowanych lub likwidowanych urządzeń ze spisu urządzeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564344"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemy z usuwaniem wyeksłowanych lub likwidowanych urządzeń ze spisu urządzeń

Usługa Microsoft Defender for Endpoint obecnie nie pozwala na ręczne usuwanie rekordu urządzenia wyzysłowego lub likwidowanego z wykazu urządzeń.

Ze względów bezpieczeństwa urządzenie pozostaje w portalu jako rekord historyczny przez maksymalnie 180 dni. Jednak dane urządzenia są czyszowane zgodnie ze skonfigurowanym okresem przechowywania.

**Uwaga:** Urządzenie wyeksłowane lub  likwidowane jest automatycznie przełączane do stanu nieaktywnego po upływie siedmiu dni. Ponadto urządzenia, które nie są aktywne w ciągu ostatnich 30 dni, nie są odzwierciedlane w danych, które odzwierciedlają twoją organizację Zarządzanie zagrożeniami i lukami wyników ekspozycji lub bezpiecznego wyniku działania firmy Microsoft dla urządzeń.
 
Jeśli nadal nie chcesz wyświetlać niektórych urządzeń w widoku Spis urządzeń, spróbuj użyć tagu urządzenia w celu odfiltrowanie zlikwidowanych urządzeń w widoku Spis urządzeń.

Aby uzyskać więcej informacji, zobacz:

[Urządzenia wye webboard z usługi Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Wynik ekspozycji w Zarządzanie zagrożeniami i lukami](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Naprawianie czujników o złej kondycji w programie Microsoft Defender dla punktu końcowego](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Jak efektywnie korzystać z otagowania (część 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Jak efektywnie korzystać z otagowania (część 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Jak efektywnie korzystać z otagowania (część 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




