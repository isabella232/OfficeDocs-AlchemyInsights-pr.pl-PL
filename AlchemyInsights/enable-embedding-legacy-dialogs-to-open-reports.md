---
title: Włączanie osadzania starszych okien dialogowych w celu otwierania raportów
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814274"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Włączanie osadzania starszych okien dialogowych w celu otwierania raportów

**Symptom**

Użytkownicy nie mogą otwierać raportów. "Coś poszło nie tak. Aby uzyskać więcej szczegółowych informacji, zapoznaj się ze szczegółami technicznymi".

**Przyczyna**

Raporty nie są ładowane w u użytkownika UCI z błędem "Deskryptor formularza ma wartość null lub nie został zdefiniowany". Raporty w układzie UCI nadal wymagają starszych okien dialogowych, więc system klienta musi mieć włączoną *funkcjęlegacydialogsembedding.*

**Rozwiązanie**

1. Przejdź do **karty >ustawienia > ustawienia systemu > Ogólne.**

2. Ustaw wartość "Włącz osadzanie niektórych starszych okien dialogowych w kliencie przeglądarki Unified Interface" na **wartość Tak.**
