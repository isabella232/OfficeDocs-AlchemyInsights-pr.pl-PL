---
title: Wskaźniki nie działają przy użyciu przeglądarki Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326271"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Wskaźniki nie działają przy użyciu przeglądarki Edge

Po utworzeniu wskaźnika nie jest on ujmowany w edge (Smartscreen). Aby uzyskać więcej informacji, zobacz Tworzenie wskaźników adresów [IP oraz adresów URL/domen.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Krok 1. Upewnij się, że są

- Sprawdź, czy wskaźnik jest poprawny (nie literówki w adresie IP/adresie URL, prawidłowa akcja, właściwe grupy RBAC).
- Poczekaj co najmniej 2 godziny po utworzeniu wskaźnika, aby uwzględnić wszelkie możliwe opóźnienia.
- Upewnij się, że system(-y) jest wnoszony do programu Microsoft Defender for Endpoint.
- Sprawdź, czy system(y) może komunikować się z chmurą.
- Sprawdź, czy filtr Smartscreen jest włączony i osiągalny, przechodząc do [witryny testowej.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Krok 2. Rozwiązywanie potencjalnego problemu

- Upewnij się, że klient spełnia wymagania. Aby uzyskać szczegółowe informacje, [zobacz Tworzenie wskaźników adresów IP oraz adresów URL/domen.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Upewnij się, że używasz najnowszej wersji przeglądarki Edge. Aby dowiedzieć się, która wersja jest najnowsza, zobacz [Dowiedz się, Microsoft Edge masz.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Uruchom ponownie przeglądarkę Edge.
- Przejdź do witryny, dla której masz wskaźnik konfiguracji. Jeśli witryna nie jest wyświetlana zgodnie z oczekiwaniami, przejdź do kroku 3. 

## <a name="step-3-collect-data"></a>Krok 3. Zbieranie danych

- Zbierz **dane diagnostyczne MDEClientAnalyzer.** Aby uzyskać instrukcje, [zobacz Problemy z komputerami dołączania do programu Microsoft Defender dla punktu końcowego.](issues-with-onboarding-machines.md)
- Jeśli wiesz, jak instalować i zbierać dane śledzenia fiddlera, zobacz [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Jeśli wolisz wskazówki z pomocy technicznej firmy Microsoft, wybierz ikonę Pomoc techniczna poniżej, aby otworzyć sprawę pomocy technicznej.
