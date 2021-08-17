---
title: MC210173 — wycofanie nowej niestandardowej funkcji formularza programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077674"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 — wycofanie nowej niestandardowej funkcji formularza programu SharePoint Designer

Zidentyfikowaliśmy problem wpływającym na funkcjonalność programu SharePoint Designer dla [tworzenia formularzy niestandardowych](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) w usłudze SharePoint Online. Po przeprowadzeniu starannej analizy stwierdziliśmy, że nie ma znanych poprawek dla tego problemu i postanowiliśmy wyłączyć funkcję tworzenia formularzy niestandardowych o godzinie 3:00 (czasu UTC) w sobotę 25 kwietnia 2020 r. Ta zmiana nie ma wpływu na możliwość edytowania wcześniej utworzonych formularzy ani innych istniejących funkcji w usłudze SharePoint Online Designer.

Po wprowadzeniu tej zmiany użytkownicy mogli otrzymać błąd: „Nie można zapisać zmian na liście na serwerze” podczas tworzenia nowych formularzy.

Użytkownicy, którzy wcześniej korzystali z programu SharePoint Designer do tworzenia formularzy niestandardowych, mogą użyć do tego celu usługi [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

Usługa PowerApps to łatwe w użyciu zaawansowane narzędzie pozwalające użytkownikom pracującym w środowisku SharePoint Online Modern tworzyć i edytować niestandardowe formularze dla list programu SharePoint i bibliotek dokumentów bezpośrednio z okna przeglądarki. Usługa PowerApps nie wymaga znajomości tradycyjnego kodowania ani pobierania żadnych dodatkowych aplikacji, takich jak program InfoPath.

**Uwaga**: użytkownicy usługi SharePoint Online Classic będą musieli chwilowo przełączać się do nowoczesnego środowiska, aby uzyskać dostęp do usługi PowerApps i korzystać z niej. Chociaż wszystkie formularze niestandardowe utworzone w usłudze PowerApps są dostępne dla doświadczonych użytkowników usługi SharePoint Online w wersji klasycznej.
