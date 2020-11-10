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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982486"
---
# <a name="comments-on-list-items"></a>Komentarze dotyczące elementów listy

Użytkownicy wkrótce będą mogli dodawać i usuwać komentarze do elementów listy. Użytkownicy mogą wyświetlać wszystkie komentarze w elemencie listy i filtrować między widokami pokazującymi komentarze lub działania związane z elementem.

**Chronometraż** :

**Wersja ukierunkowana** : stopniowe przewinięcie w połowie października i oczekiwanie na zakończenie w połowie listopada

**Wersja Standard** : stopniowe przewinięcie w połowie listopada i oczekiwanie na zakończenie przed dniem grudnia

**Wprowadzanie** : wersja ukierunkowana dla całej organizacji

Aby można było dodawać i usuwać komentarze, użytkownicy muszą zwrócić uwagę na następujące kwestie:

- Komentarze są zgodne z ustawieniami uprawnień w programie SharePoint.
- Listy klasyczne, które nie są jeszcze zbudowane do wyświetlania w nowoczesnych interfejsach użytkowników, na przykład listy zadań, nie będą miały tej funkcji komentowania.
- Komentowanie list w aplikacji Teams nie jest dostępne w tej wersji.
- Komentarze nie są indeksowane przez wyszukiwanie.

Administratorzy mogą wyłączyć tę funkcję na poziomie organizacji, zmieniając parametr **CommentsOnListItemsDisabled** w poleceniu cmdlet **Set-SPOTenant** programu PowerShell.

Obecnie nie można wyłączyć komentowania na poziomie witryny lub listy. Mamy nadzieję, że te kontrolki będą znajdować się w nowszej aktualizacji, prawdopodobnie w pierwszym kwartale 2021.
