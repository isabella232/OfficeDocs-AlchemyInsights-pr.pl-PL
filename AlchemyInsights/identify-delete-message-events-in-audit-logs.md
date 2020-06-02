---
title: Identyfikowanie zdarzeń usuwania wiadomości w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508998"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dzienniki inspekcji usuniętych wiadomości e-mail

Począwszy od stycznia 2019 r., firma Microsoft domyślnie włącza rejestrowanie inspekcji skrzynek pocztowych. W przeciwnym razie, aby przejrzeć zdarzenia usuwania wiadomości dla określonego użytkownika, należy ręcznie włączyć akcje usuwania do inspekcji. Jeśli rejestrowanie inspekcji skrzynki pocztowej jest już włączone dla twojej organizacji lub dla określonego użytkownika, wykonaj poniższe czynności.

1. Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/)

2. Kliknij **pozycję Wyszukaj i przeszukuj** i wybierz pozycję **Wyszukiwanie dziennika inspekcji**.

3. Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia.** Określ nazwę użytkownika, który chcesz zbadać (użytkownik, który usunął elementy). W polu **Działania** wybierz folder **Usunięte wiadomości z folderu Elementy usunięte** i folder **Przeniesiono wiadomości do folderu Elementy usunięte**.

4. Kliknij **pozycję Wyszukaj**.

W wynikach wybierz rekord inspekcji. W wysu wysu wysu wysunął szczegóły kliknij pozycję **Więcej informacji**. Dodatkowe informacje o usuniętym elemencie (na przykład wiersz tematu i lokalizacja elementu, gdy został usunięty) są wyświetlane w polu **AffectedItems.** **Właściwość ClientInfoString** zostanie wyświetlena, jeśli usunięcie nastąpiło w programie Outlook, w programie Outlook w sieci Web (wcześniej znanej jako outlook web app) lub na jakimkolwiek innym urządzeniu.

Aby uzyskać więcej informacji, zobacz [Określanie, kto skonfigurował przekazywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Uwaga:** Nie można pobrać usuniętych elementów przy użyciu funkcji dziennika inspekcji. Aby pobrać usunięte wiadomości w aplikacji Outlook w sieci Web, zobacz [Odzyskiwanie usuniętych elementów w aplikacji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
