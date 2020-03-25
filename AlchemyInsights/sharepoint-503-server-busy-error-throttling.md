---
title: Ograniczanie przepustowości usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931236"
---
# <a name="sharepoint-online-throttling"></a>Ograniczanie przepustowości usługi SharePoint Online

**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle. Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych. W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.

W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia. Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach. Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.

**Serwer 503 jest zajęty błąd**

Użytkownicy mogą otrzymać błąd 503 serwer jest zajęty podczas próby przejścia do witryn programu SharePoint lub OneDrive. 

Ten błąd może być spowodowany przez ograniczanie przepustowości w usłudze sharepoint. Usługa SharePoint Online używa ograniczania przepustowości w celu zachowania optymalnej wydajności i niezawodności usługi SharePoint Online. Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (według skryptu lub kodu), aby zapobiec nadużywaniu zasobów. 

Aby uzyskać więcej informacji na temat ograniczania przepustowości, [zobacz: Unikanie ograniczania lub blokowania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Jeśli uważasz, że ten błąd nie jest związany z ograniczaniem przepustowości, możesz sprawdzić, czy w dzierżawie występuje aktywna konserwacja, przechodząc do [Centrum wiadomości.](https://portal.office.com/adminportal/home#/MessageCenter)

 Na koniec upewnij się, że odwiedź [service health](https://portal.office.com/adminportal/home#/servicehealth) strony, aby sprawdzić, czy wszelkie porady /incydenty, które mogą wystąpić.

