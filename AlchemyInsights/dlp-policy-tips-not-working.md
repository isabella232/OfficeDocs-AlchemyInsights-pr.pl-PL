---
title: Porady dotyczące zasad DLP nie działają
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932596"
---
# <a name="dlp-policy-tip-issues"></a>Problemy z poradami dotyczącymi zasad DLP

**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle. Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych. W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.

W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia. Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach. Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.

**Wskazówki dotyczące zasad DLP**

Podczas korzystania z **zasad DLP**użytkownicy mogą otrzymywać powiadomienia o naruszeniu zasad za pomocą **wskazówek dotyczących zasad.** Administratorzy mogą skonfigurować wskazówki dotyczące zasad do wyświetlania podczas testowania zasad DLP lub gdy zasady są w trybie pełnego wymuszania.
  
Aby skonfigurować wskazówki dotyczące zasad dotyczących zasad DLP w Centrum zabezpieczeń i zgodności w trybie pełnego wymuszania, wykonaj następujące czynności:
  
- Upewnij się, że wskazówki dotyczące zasad zostały **włączone** w regule DLP, wykonując kroki [opisane w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Upewnij się, że **zawartość jest zgodna** z tym, co jest **wymagane** do wyzwolenia reguły opisanej w tym artykule [tutaj](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Porady dotyczące zasad są wyświetlane zarówno w programie OWA, jak i w programie Outlook. Jednak w przypadku korzystania z **programu Outlook 2013 lub nowszego**porady dotyczące zasad są wyświetlane tylko pod pewnymi warunkami. Te warunki są wymienione w tym miejscu: [Obsługiwane warunki dla programu Outlook 2013 lub nowszego dotyczące wyświetlania porad dotyczących zasad](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Aby uzyskać dodatkowe informacje na temat wskazówek dotyczących zasad DLP, zobacz: [Pokaż wskazówki dotyczące zasad dla zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  