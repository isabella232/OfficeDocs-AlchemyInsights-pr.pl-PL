---
title: Komentarze dotyczące elementów listy
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
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995497"
---
# <a name="comments-on-list-items"></a>Komentarze dotyczące elementów listy

Użytkownicy mogą wyświetlać wszystkie komentarze dotyczące elementu listy i filtrować widok między widokami, w których są wyświetlane komentarze lub działania związane z elementem.

Użytkownicy muszą zanotować następujące informacje, zanim będą oni mieli możliwość dodawania i usuwania komentarzy:

- Komentarze są zgodne z ustawieniami uprawnień, które są SharePoint.
- Klasyczne listy, które nie są jeszcze wbudowane w nowoczesne interfejsy użytkownika, takie jak listy zadań, nie będą zawierały tej funkcji do komentowania.
- Komentowanie list w programie Teams jest niedostępne w tej wersji.
- Komentarze nie są indeksowane przez wyszukiwanie.

Administratorzy mogą wyłączyć tę funkcję na poziomie organizacji, zmieniając parametr **CommentsOnListItemsDisabled** w polu cmdlet programu PowerShell **Set-SPOTenant.**

Obecnie nie można wyłączyć komentowania na poziomie witryny lub listy. Mamy nadzieję, że te kontrolki będą się liczyć w późniejszej aktualizacji, prawdopodobnie w pierwszym kwartale 2021 roku.
