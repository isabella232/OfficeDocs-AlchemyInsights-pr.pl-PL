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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724164"
---
# <a name="comments-on-list-items"></a>Komentarze dotyczące elementów listy

Użytkownicy mogą wyświetlać wszystkie komentarze w elemencie listy i filtrować między widokami pokazującymi komentarze lub działania związane z elementem.

Aby można było dodawać i usuwać komentarze, użytkownicy muszą zwrócić uwagę na następujące kwestie:

- Komentarze są zgodne z ustawieniami uprawnień w programie SharePoint.
- Listy klasyczne, które nie są jeszcze zbudowane do wyświetlania w nowoczesnych interfejsach użytkowników, na przykład listy zadań, nie będą miały tej funkcji komentowania.
- Komentowanie list w aplikacji Teams nie jest dostępne w tej wersji.
- Komentarze nie są indeksowane przez wyszukiwanie.

Administratorzy mogą wyłączyć tę funkcję na poziomie organizacji, zmieniając parametr **CommentsOnListItemsDisabled** w poleceniu cmdlet **Set-SPOTenant** programu PowerShell.

Obecnie nie można wyłączyć komentowania na poziomie witryny lub listy. Mamy nadzieję, że te kontrolki będą znajdować się w nowszej aktualizacji, prawdopodobnie w pierwszym kwartale 2021.
