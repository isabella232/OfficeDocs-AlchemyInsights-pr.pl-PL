---
title: Usuwanie danych i czyszczenie urządzeń w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331051"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Usuwanie danych i czyszczenie urządzeń w usłudze Intune

Zdalne akcje Wycofywanie urządzenia i Czyszczenie urządzenia mogą być używane do usuwania danych firmowych zarządzanych przez usługę Intune lub do zresetowania urządzenia do ustawień fabrycznych i przywrócenia ustawień domyślnych.

1. Zaloguj się do usługi zarządzania urządzeniami na platformie Microsoft 365 i przejdź do opcji **Urządzenia** > **Wszystkie urządzenia**.
2. Wybierz urządzenie, które chcesz wyczyścić.
3. Wybierz wymagany typ zdalnego czyszczenia. Opcja Wycofywanie usuwa tylko informacje o organizacji, podczas gdy pełne czyszczenie przywraca urządzenie do ustawień fabrycznych.
4. Wybierz pozycję **Tak**, aby potwierdzić. Do czasu ukończenia czyszczenia status akcji urządzenia wyświetla się jako *Wycofywanie w toku*.
    Po zakończeniu akcji nie zobaczysz urządzenia przenośnego na liście urządzenia zarządzanego. 

**Uwaga:** Danych firmowych nie można usunąć z urządzeń PRZYŁĄCZNYCH DO USŁUGI Azure AD. 

Aby uzyskać szczegółowe informacje na temat skutków akcji wycofywania i czyszczenia, w tym to, co zostało zachowane, a co usunięte, zobacz następującą dokumentację:

- [Usuwanie urządzeń przy użyciu czyszczenia, wycofywania lub ręcznego wyrejestrowywania urządzenia](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Jak czyścić z aplikacji usługi Intune tylko dane firmowe](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Usuwanie wszystkich danych z urządzenia z systemem macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).