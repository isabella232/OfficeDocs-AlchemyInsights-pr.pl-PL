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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003399"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Włączanie osadzania starszych okien dialogowych w celu otwierania raportów

**Objaw**

Użytkownicy nie mogą otwierać raportów. "Coś poszło nie tak. Aby uzyskać więcej szczegółowych informacji, zapoznaj się ze szczegółami technicznymi".

**Przyczyna**

Raporty nie są ładowane w u użytkownika UCI z błędem "Deskryptor formularza ma wartość null lub nie został zdefiniowany". Raporty w układzie UCI nadal wymagają starszych okien dialogowych, więc system klienta musi mieć włączoną *funkcjęlegacydialogsembedding.*

**Rozwiązanie**

1. Przejdź do **Ustawienia >administracji > systemowej Ustawienia > karcie Ogólne.**

2. Ustaw wartość "Włącz osadzanie niektórych starszych okien dialogowych w kliencie przeglądarki Unified Interface" na **wartość Tak.**
