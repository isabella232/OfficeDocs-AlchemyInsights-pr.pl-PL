---
title: Nie można dodać konta po uaktualnieniu do systemu macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506752"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nie można dodać konta po uaktualnieniu do systemu macOS 11.6 Big Sur

Po uaktualnieniu do systemu macOS 11.6 OneDrive dla konta służbowego lub osobistego programu OneDrive może nie być widoczne na liście kont i możesz nie być w stanie zalogować się do drugiego konta z aplikacji.

Opracowaliśmy poprawkę dla tego problemu. Najpierw określ, czy używasz autonomicznej, czy z wersji ze sklepu App Store pakietu OneDrive:

- Wybierz chmurę OneDrive na pasku menu, aby > **pomoc & Ustawienia**  >    >  **Preferencje .** Jeśli numer wersji nie zawiera **(wersja autonomiczna)**, masz wersję tego produktu ze sklepu App Store.

Jeśli korzystasz z autonomicznej wersji pakietu OneDrive uruchom ponownie komputer i OneDrive automatyczne aktualizacje do kompilacji, w której ten problem został rozwiązany. Jeśli chcesz zainstalować kompilację ręcznie, pobierz ten plik [.zip,](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)rozpakować plik i skopiuj aplikację OneDrive do folderu Programy (zastępując istniejącą aplikacją pakietu OneDrive).

Jeśli korzystasz z wersji ze sklepu App Store, rozważ zainstalowanie autonomicznej wersji pakietu OneDrive. Ta wersja działa tak samo jak wersja ze sklepu App Store, ale umożliwia firmie Microsoft oferuje użytkownikom aktualizacje szybciej i łączy ich z wersją, która zawiera poprawkę rozsyłaną ten problem.

1. Pobierz autonomiczną wersję pakietu [OneDrive która zawiera poprawkę.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Rozpakować plik i skopiuj aplikację OneDrive do folderu Programy (zastępując istniejącą OneDrive aplikację).

Jeśli chcesz użyć wersji ze sklepu App Store, poczekaj, aż sklep App Store wyda wersję aplikacji, która zawiera poprawkę. Niestety firma Microsoft nie może zakomunikować szacowanej daty wydania ustalonej wersji ze sklepu App Store.


