---
title: Stan czujnika sprawdzania punktu końcowego programu Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676341"
---
# <a name="defender-endpoint-check-sensor-status"></a>Stan czujnika sprawdzania punktu końcowego programu Defender

Kafelek **Urządzenia z problemami z** czujnikiem znajduje się na pulpicie nawigacyjnym Operacje zabezpieczeń. Ten kafelek zawiera informacje o możliwościach poszczególnych urządzeń w celu przekazywania danych czujnika i komunikowania się z usługą Defender for Endpoint. Raportuje ono, ile urządzeń wymaga uwagi i ułatwia zidentyfikowanie urządzeń sprawiających problem oraz podejmie działania w celu poprawienia znanych problemów.

Dwa wskaźniki stanu na kafelku zapewniają informacje o liczbie urządzeń, które nie zgłaszają poprawnie usługi:

- **Błędnie skonfigurowane** Urządzenia, które mogą częściowo raportować dane czujnika do usługi Defender for Endpoint i mogą mieć błędy konfiguracji, które wymagają korekty.
- **Nieaktywny** Urządzenia, które w ciągu ostatniego miesiąca przestały zgłaszać się do usługi Defender for Endpoint przez ponad siedem dni.

Kliknięcie dowolnej grupy pokieruje Cię do listy Urządzenia przefiltrowane według twoich opcji. Na liście Urządzenia możesz filtrować listę stanu kondycji według następującego stanu:

- **Aktywny** Urządzenia, które aktywnie zgłaszają się do usługi Defender for Endpoint.
- **Błędnie skonfigurowane** Urządzenia, które mogą częściowo raportować dane czujnika do usługi Defender for Endpoint, ale mają błędy konfiguracji, które trzeba poprawić. Błędnie skonfigurowane urządzenia mogą mieć jeden lub połączenie następujących problemów:

    - Brak danych czujnika — urządzenia przestały wysyłać dane czujnika. Z urządzenia można wyzwolić ograniczone alerty.
    - Ograniczona komunikacja — możliwość komunikowania się z urządzeniem jest ograniczona. Wysyłanie plików do dogłębnej analizy, blokowanie plików, odizolowanie urządzenia od sieci i inne akcje, które wymagają komunikacji z urządzeniem, mogą nie działać.
- **Nieaktywny** Urządzenia, które przestały zgłaszać się do usługi Defender for Endpoint.

Za pomocą funkcji Eksportowanie możesz pobrać całą listę w formacie CSV.

Aby uzyskać więcej informacji, [zobacz Sprawdzanie stanu kondycji czujnika w programie Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Aby uzyskać więcej informacji o tym, co spowodowało, że urządzenie było nieaktywne lub nieprawidłowo skonfigurowane, zobacz Naprawianie czujniki o złej kondycji w programie [Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
