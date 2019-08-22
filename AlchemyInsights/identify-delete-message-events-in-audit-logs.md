---
title: Identyfikowanie Usuń wiadomość zdarzeń w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539219"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dzienniki inspekcji dla usunięte wiadomości e-mail

Począwszy od stycznia 2019, Microsoft jest włączenie rejestrowania domyślnie inspekcji skrzynki pocztowej. W przeciwnym razie Aby przejrzeć delete komunikat zdarzenia dla określonego użytkownika, należy ręcznie włączyć akcje usuwania w celu prowadzenia inspekcji. Jeśli skrzynka pocztowa inspekcji rejestrowanie jest już włączone dla danej organizacji lub dla określonego użytkownika, wykonaj następujące kroki.

1. Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/)

2. Kliknij przycisk **Wyszukaj i dochodzenia** i wybierz **Przeszukiwania dzienników inspekcji**.

3. Wybierz zakres dat w polach **Data początkowa** i **Data końcowa** . Umożliwia określenie nazwy użytkownika dla użytkownika, który chcesz zbadać (użytkownik, który elementy usunięte). W dziedzinie **działalności** wybierz opcję **usunięte wiadomości z folderu Elementy usunięte** i **wiadomości przenoszonych do folderu Elementy usunięte**.

4. Kliknij przycisk **Wyszukaj**.

W wynikach wybierz rekord audytu. W menu wysuwane Szczegóły kliknij przycisk **Więcej informacji**. Dodatkowe informacje o usunięty element (na przykład, wiersz tematu i lokalizacji elementu, gdy został usunięty) jest wyświetlana w polu **AffectedItems** . Właściwość **ClientInfoString** pokaże, czy usunięcie pojawił się w programie Outlook, program Outlook w sieci web (dawniej znany jako aplikacji sieci Web programu Outlook) lub inne urządzenie.

Aby uzyskać więcej informacji zobacz [Określanie, która skonfigurowała przekazywanie dla skrzynki pocztowej wiadomości e-mail](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Uwaga**: nie można pobrać elementy usunięte za pomocą funkcji dziennika inspekcji. Aby odzyskać usunięte wiadomości w programie Outlook w sieci web, zobacz [Odzyskiwanie usuniętych elementów w programie Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
