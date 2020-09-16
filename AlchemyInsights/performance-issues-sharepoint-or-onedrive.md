---
title: Problemy z wydajnością — program SharePoint lub usługa OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771911"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Program SharePoint lub usługa OneDrive jest wolny, niedostępny lub niedostępny dla wielu użytkowników

Program SharePoint lub usługa OneDrive może być wolny, niedostępny lub niedostępny albo może wyświetlać niedostępną usługę lub 503 błędy z kilku powodów:
  
- Jeśli witryna programu SharePoint lub usługi OneDrive jest powolna lub opóźniona dla wielu użytkowników, może to oznaczać, że wystąpił tymczasowy problem z usługą, w którym użytkownicy mogą napotkać sporadyczne opóźnienia lub błędy nawigacji podczas uzyskiwania dostępu do witryn programu SharePoint lub zawartości OneDrive. Sprawdź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ na.
  
- Po próbie przejścia do witryny programu SharePoint lub usługi OneDrive użytkownicy mogą otrzymać komunikat o błędzie *serwera 503 jest zajęty* . Przyczyną tego błędu może być ograniczenie w ramach usługi programu SharePoint. Usługa SharePoint Online używa ograniczania, aby zapewnić optymalną wydajność i niezawodność usługi SharePoint Online. Ograniczanie ogranicza liczbę akcji użytkownika lub współbieżnych połączeń (za pomocą skryptu lub kodu), aby zapobiec nadmiernemu zużyciu zasobów. Aby uzyskać więcej informacji na temat ograniczania przepustowości, zobacz [unikanie ograniczania lub blokowania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Jeśli masz niską wydajność w **klasycznej** lub **nowoczesnej** witrynie lub stronie programu SharePoint, użyj [narzędzia Diagnostyka strony](https://aka.ms/perftool) do analizowania stron.
  
- Jeśli nadal masz ogólne wolne wyniki, zobacz zasoby na dole tego artykułu: [wprowadzenie do dostrajania wydajności usługi SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  