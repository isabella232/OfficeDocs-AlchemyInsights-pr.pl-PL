---
title: Identyfikowanie zdarzeń usuwania wiadomości w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868428"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dzienniki inspekcji usuniętych wiadomości e-mail

Od stycznia 2019 r. firma Microsoft domyślnie włączona jest rejestrowanie inspekcji skrzynki pocztowej. W przeciwnym razie, aby przejrzeć zdarzenia usuwania wiadomości dla określonego użytkownika, musisz ręcznie włączyć akcje usuwania na potrzeby inspekcji. Jeśli rejestrowanie inspekcji skrzynki pocztowej jest już włączone dla organizacji lub konkretnego użytkownika, wykonaj poniższe czynności.

1. Logowanie się do [Centrum Microsoft 365 zgodności](https://protection.office.com/)

2. Kliknij **pozycję Wyszukiwanie i badanie** i wybierz pozycję **Przeszukiwanie dziennika inspekcji**.

3. Zaznacz zakres dat w **polach Data rozpoczęcia** **i Data zakończenia.** Określ nazwę użytkownika, który chcesz zbadać (użytkownika, który usunął te elementy). W polu **Działania** zaznacz elementy usunięte wiadomości z **folderu Elementy usunięte i** Przenieś wiadomości do folderu Elementy **usunięte.**

4. Kliknij **przycisk Wyszukaj**.

W wynikach wybierz rekord inspekcji. W wysuwanych szczegółach kliknij pozycję **Więcej informacji**. W polu **Elementy** objęte problemem są wyświetlane dodatkowe informacje dotyczące usuniętego elementu (na przykład wiersz tematu i lokalizacja usuniętego elementu). Właściwość **ClientInfoString** będzie pokazywana, jeśli usunięcie wystąpiło w programie Outlook, Outlook w sieci Web (dawniej Outlook Web App) lub innym urządzeniu.

Aby uzyskać więcej informacji, zobacz Określanie, kto s skonfigurować [przesyłanie dalej poczty e-mail dla skrzynki pocztowej.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Uwaga:** Za pomocą funkcji dziennika inspekcji nie można pobrać usuniętych elementów. Aby pobrać usunięte wiadomości do Outlook w sieci Web, zobacz [Odzyskiwanie usuniętych](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)elementów w aplikacji Outlook Web App.
