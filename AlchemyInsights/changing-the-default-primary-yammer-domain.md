---
title: Zmiana domyślnej domeny usługi Yammer
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
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950126"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Zmiana domyślnej lub podstawowej domeny usługi Yammer

Adres URL usługi Yammer zawiera nazwę bieżącej domeny podstawowej dla Twojej sieci Yammer. Ta nazwa domeny może nie pokrywać się z nazwą domeny podstawowej ustawioną w usłudze Office 365 lub Azure AD. Działanie będzie się różnić w zależności od liczby domen niestandardowych dodanych do dzierżawy i od tego, czy usługa Yammer jest w obsługiwanej konfiguracji (1 dzierżawa: 1 sieć lub 1:1). Dostępne są materiały dotyczące [domen usługi Yammer i Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Najczęstszą przyczyną wyświetlania się nieprawidłowej domeny jest istnienie wielu sieci Yammer i konieczność ich konsolidacji. [Konsolidacja do jednej sieci](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)za pomocą narzędzia migracji sieci to ważny pierwszy krok. Należy go wykonać przed próbą ustawienia domeny podstawowej.

**Brak domen niestandardowych**

W przypadku nowych dzierżaw w usłudze Yammer będzie używana domyślna domena (np. fabrikam.onmicrosoft.com) z danej dzierżawy. Domena podstawowa jest ustawiona jako yammer.com/fabrikam.onmicrosoft.com.

**Pojedyncza domena niestandardowa**

W usłudze Yammer domena niestandardowa (np. fabrikam.com) z danej dzierżawy zostanie automatycznie wybrana jako domena podstawowa dla usługi Yammer. Jest ona ustawiona jako yammer.com/fabrikam.com. Wprowadzanie tej zmiany ma miejsce w ramach usługi synchronizacji domeny i zajmuje do 24 godzin.

**Wiele domen niestandardowych**

Domena podstawowa w usłudze Yammer może różnić się od domyślnej domeny dzierżawy. W przypadku istnienia wielu domen niestandardowych usługa Yammer nie dokonuje prób ustalenia, która z dostępnych domen jest prawidłowa. Aby poprosić o zmianę nazwy domeny podstawowej na wybraną domenę podstawową, konieczne jest przesłanie zgłoszenia do działu pomocy technicznej.

**Dodatkowe informacje na temat rozwiązywania problemów**

W niektórych przypadkach domeny mogły zostać przeniesione między dzierżawami, a usługa synchronizacji domen nie zadziałała poprawnie. W tym wypadku poza nieprawidłową domeną podstawową mogą wystąpić dodatkowe problemy, w tym z logowaniem. Aby rozwiązać ten problem, konieczne może być przeniesienie domen do prawidłowej sieci przy asyście działu pomocy technicznej firmy Microsoft. W takiej sytuacji konieczne jest uzyskanie bezpośredniej pomocy, a rozwiązanie problemu może zająć trochę czasu, zwłaszcza jeśli lista nazw domen jest bardzo długa. Aby uzyskać pomoc w tego typu sytuacji, wyślij zgłoszenie do działu pomocy technicznej.

Agent działu pomocy technicznej sprawdzi, czy domeny w ramach dzierżawy pozostającej pod Twoją kontrolą są zweryfikowane. Jeśli domeny zostały dodane do Twojej dzierżawy, ale nie zostały zweryfikowane w systemie DNS, agent może zadać dodatkowe pytania w celu przeprowadzenia weryfikacji.  Aby usprawnić proces, zadbaj o weryfikację domen w systemie DNS.
