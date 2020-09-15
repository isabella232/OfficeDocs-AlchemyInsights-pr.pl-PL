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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696523"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dzienniki inspekcji dla usuniętych wiadomości e-mail

Począwszy od stycznia 2019 r., firma Microsoft domyślnie Włącza rejestrowanie inspekcji skrzynek pocztowych. W przeciwnym razie, aby przejrzeć zdarzenia usuwania wiadomości dla określonego użytkownika, należy ręcznie włączyć inspekcję akcji usuwania. Jeśli rejestrowanie inspekcji skrzynki pocztowej jest już włączone dla Twojej organizacji lub dla określonego użytkownika, wykonaj poniższe czynności.

1. Logowanie się do [Centrum zgodności & programu Microsoft 365 Security](https://protection.office.com/)

2. Kliknij pozycję **Wyszukiwanie i badanie** , a następnie wybierz pozycję **Wyszukiwanie dziennika inspekcji**.

3. Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia** . Określ nazwę użytkownika, który ma zostać zbadany (użytkownik, który usunął elementy). W polu **działania** wybierz pozycję **usunięte wiadomości z folderu Elementy usunięte** i **Przenieś wiadomości do folderu Elementy usunięte**.

4. Kliknij przycisk **Wyszukaj**.

W wynikach wybierz rekord inspekcji. W menu wysuwanym Szczegóły kliknij pozycję **więcej informacji**. Dodatkowe informacje na temat usuniętego elementu (na przykład wiersza temat i lokalizacji elementu, w którym został on usunięty) są wyświetlane w polu **AffectedItems** . W przypadku wystąpienia usunięcia w programie Outlook, aplikacji Outlook w sieci Web (dawniej nazywanej aplikacją Outlook Web App) zostanie wyświetlona Właściwość **ClientInfoString** lub inne urządzenie.

Aby uzyskać więcej informacji, zobacz [Określanie, kto konfiguruje przekierowywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Uwaga**: elementy usunięte nie mogą być pobierane przy użyciu funkcji dziennika inspekcji. Aby pobrać usunięte wiadomości w aplikacji Outlook w sieci Web, zobacz [odzyskiwanie elementów usuniętych w aplikacji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
