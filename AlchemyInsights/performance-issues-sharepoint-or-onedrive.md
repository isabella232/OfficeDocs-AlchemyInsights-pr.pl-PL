---
title: Problemy z wydajnością SharePoint lub OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911852"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint lub OneDrive wolne, niedostępne lub niedostępne dla wielu użytkowników

SharePoint lub OneDrive mogą być wolne, niedostępne, niedostępne lub mogą powodować wyświetlanie komunikatów o błędach usługi niedostępnych lub 503 z kilku powodów:
  
- Jeśli witryna usługi SharePoint lub OneDrive jest wolna lub opóźniona u wielu użytkowników, może wystąpić tymczasowy problem z usługą, gdy użytkownicy występują sporadyczne opóźnienia lub błędy nawigacji podczas uzyskiwania dostępu do witryn SharePoint lub zawartości OneDrive sieci OneDrive. Sprawdź na [pulpicie nawigacyjnym](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) Kondycja usługi, czy wpływa to na Twoją organizację.
  
- Użytkownicy mogą otrzymać błąd *"Serwer 503* jest zajęty" podczas próby przechodzenia do SharePoint lub OneDrive witryn. Ten błąd może być spowodowany przez ograniczanie w obrębie SharePoint sieci. Usługa SharePoint Online używa ograniczania, aby zapewnić optymalną wydajność i niezawodność usługi SharePoint Online. Ograniczanie ogranicza liczbę akcji użytkownika lub współbieżnych połączeń (za pomocą skryptu lub kodu), aby zapobiec nadmiernemu zużyciu zasobów. Aby uzyskać więcej informacji na temat ograniczania, zobacz Unikanie ograniczania lub blokowania w u [SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Jeśli masz wolne działanie w  przypadku **klasycznej** lub SharePoint witryny [](https://aka.ms/perftool) lub strony, przeanalizuj strony za pomocą narzędzia diagnostycznego stron.
  
- Jeśli nadal masz wolne działanie, zapoznaj się z zasobami u dołu tego artykułu: Wprowadzenie do dostosowywania wydajności dla usługi [SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  