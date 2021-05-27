---
title: Brakuje spisu oprogramowania lub niedokładne informacje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676510"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Brakuje spisu oprogramowania lub niedokładne informacje

Spis oprogramowania w aplikacji Zarządzanie zagrożeniami i lukami to lista znanego oprogramowania w organizacji z oficjalnymi wyliczeniami wspólnej platformy (CPE, Common Platform Enumerations).

Produkty oprogramowania bez oficjalnego cpe nie mają opublikowanych luk w zabezpieczeniach. W spisie znajdują się również szczegółowe informacje, takie jak imię i nazwisko dostawcy, liczba braków, zagrożenia i liczba dostępnych urządzeń.

Zmiany oprogramowania na urządzeniach są zazwyczaj odzwierciedlane w portalach zabezpieczeń w ciągu dwóch godzin. Jednak czasami może to trwać dłużej. Obecnie nie można wymusić synchronizacji. jest to ciągła ocena.

Jeśli po 5 godzinach zmiany oprogramowania w programie tvm nie są dokładnie odzwierciedlane, wykonaj następujące czynności:

1. Zapoznaj się z sekcją dowodów na temat oprogramowania, aby dowiedzieć się, jak wykryto oprogramowanie.
1. Upewnij się, że oprogramowanie jest obsługiwane. Oprogramowanie może być widoczne tylko na poziomie urządzenia, nawet jeśli nie jest obecnie obsługiwane przez Zarządzanie zagrożeniami i lukami. Dostępne są jednak tylko ograniczone dane.
1. Aby uzyskać instrukcje dotyczące zgłaszania nieścisłości z portalu, zobacz Zgłaszanie [nieścisłości.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Uwaga:** Zgłaszanie nieścisłości z portalu MDE to jednokierunkowy kanał dla inżynierów. Jeśli ten problem jest pilny, otwórz bilet pomocy technicznej.

Aby uzyskać więcej informacji, zobacz [Spis Zarządzanie zagrożeniami i lukami.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)