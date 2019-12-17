---
title: Problemy z wydajnością-SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068422"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint lub OneDrive powolne, niedostępne lub niedostępne dla wielu użytkowników

SharePoint lub OneDrive może być powolne, niedostępne lub niedostępne lub mogą być wyświetlane usługi niedostępne lub 503 błędy, z kilku powodów:
  
- Jeśli witryny programu SharePoint lub OneDrive jest powolne lub opóźnione dla wielu użytkowników, może być problem tymczasowy usługi, gdzie użytkownicy wystąpić sporadyczne opóźnienia lub błędy nawigacji podczas uzyskiwania dostępu do witryn programu SharePoint lub zawartości OneDrive. Sprawdź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby zobaczyć, jeśli Twoja organizacja ma wpływ.
  
- Użytkownicy mogą otrzymać *503 serwer jest zajęty* błąd podczas próby przejdź do witryny programu SharePoint lub OneDrive. Ten błąd może być spowodowany przez ograniczanie przepustowości w ramach usługi programu SharePoint. Usługa SharePoint Online używa ograniczania przepustowości, aby zachować optymalną wydajność i niezawodność usługi SharePoint Online. Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (przez skrypt lub kod), aby zapobiec nadmiernym użyciu zasobów. Aby uzyskać więcej informacji na temat ograniczania przepustowości Zobacz, [Unikaj uzyskiwania ograniczane lub zablokowane w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Jeśli wydajność pracy jest niska w **klasycznej** lub **nowoczesnej** witrynie lub na stronie programu SharePoint, użyj [narzędzia diagnostycznego strony](https://aka.ms/perftool) do analizowania stron.
  
- Jeśli nadal występują ogólne niska wydajność, zapoznaj się z zasobami na dole tego artykułu: [wprowadzenie do dostrajania wydajności programu SharePoint w trybie online](https://go.microsoft.com/fwlink/?linkid=2024334)
  