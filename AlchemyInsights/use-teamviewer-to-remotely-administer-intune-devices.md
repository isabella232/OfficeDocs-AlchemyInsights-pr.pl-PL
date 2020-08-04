---
title: Zdalne administrowanie urządzeniami usługi Intune za pomocą funkcji TeamViewer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555244"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Zdalne administrowanie urządzeniami usługi Intune za pomocą funkcji TeamViewer

Urządzenia zarządzane przez usługę Intune mogą być administrowane zdalnie za pomocą [programu TeamViewer](https://www.teamviewer.com/).

Aby administrować usłudze Intune przy użyciu programu TeamViewer, wykonaj następujące czynności: 

Rozpocznij od uzyskania poświadczeń od programu TeamViewer, aby skonfigurować łącznik TeamViewer w usłudze Intune. Dzięki temu administrator może wprowadzić poświadczenia w interfejsie użytkownika łącznika teamviewer w obszarze Urządzenia, jednorazowa operacja w celu ustanowienia łącza między usługą Intune i usługą TeamViewer.

**Część 1: Rozpoczęcie sesji za pomocą urządzenia zdalnego**

1. W obszarze **Wszystkie urządzenia**wybierz urządzenie, z którego chcesz rozpocząć sesję zdalną.
2. Od **... Więcej**, wybierz **pozycję Nowa sesja pomocy zdalnej**.
3. Wybierz **pozycję Tak,** aby potwierdzić, że chcesz ustanowić sesję zdalną.
    Po potwierdzeniu żądania "Inicjowanie nowej sesji zdalnej" przez usługę TeamViewer zostanie wyświetlona opcja **Uruchom pomoc zdalną** pod szczegółowymi informacjami o okienku Przegląd (lub Essentials) dla urządzenia. Wybierz **pozycję Zobacz więcej,** aby rozwinąć okienko i wyświetlić stan Pomocy zdalnej.
4. Wybierz **pozycję Rozpocznij sesję zdalną,** aby zainicjować sesję po stronie administratora.
5. Wybierz, aby pobrać plik binarny TeamViewer (Windows) i wybierz pozycję **Uruchom**.<br/>
    **Uwaga** Możesz zignorować dowolną stronę przeglądarki internetowej otwartą na stronie internetowej TeamViewer.

6. Potwierdź żądanie aplikacji TeamViewer, aby wprowadzić zmiany na urządzeniu (tylko windows).
7. Uruchomiono aplikację TeamViewer i zawiera kod sesji do uwierzytelniania połączenia z urządzeniem zdalnym.

**Część 2: Na urządzeniu przeznaczonym do zdalnej sesji**

1. Otwórz portal firmy usługi Intune.
2. Poszukaj flagi powiadomień: "Administrator IT żąda kontroli nad tym urządzeniem dla sesji pomocy zdalnej" i wybierz powiadomienie.
3. Wybierz, aby pobrać aplikację TeamViewer lub potwierdzić pobranie aplikacji TeamViewer ze sklepu z aplikacjami, a następnie wybierz pozycję **Uruchom**.
    **Uwaga** Możesz zignorować dowolną stronę przeglądarki internetowej otwartą na stronie internetowej TeamViewer.

4. Potwierdź żądanie aplikacji TeamViewer, aby wprowadzić zmiany na urządzeniu (tylko windows).
5. Uruchomiono aplikację TeamViewer i zawiera kod sesji do uwierzytelniania połączenia z urządzeniem zdalnym.
6. Wyskakujące okienko z pytaniem, czy chcesz zezwolić na rozpoczęcie sesji.

**Uwaga** Kody sesji generowane przez usługę TeamViewer są tylko jednorazowe. W przypadku utraty połączenia należy:

1. Zamknij wystąpienie aplikacji TeamViewer na urządzeniu zdalnym i na stacji roboczej administratora.
2. Zamknij portal firmy na urządzeniu zdalnym.
3. Inicjowanie nowej "Nowej sesji pomocy zdalnej" z portalu administracyjnego.
4. Otwórz ponownie portal firmy na urządzeniu zdalnym, aby otrzymać nowe powiadomienie.
5. Pobierz i otwórz aplikację TeamViewer zarówno na urządzeniu zdalnym, jak i na stacji roboczej administratora, tak jak poprzednio.