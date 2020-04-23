---
title: Zduplikowany rekord urządzenia w portalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790167"
---
# <a name="duplicate-device-record-in-the-portal"></a>Zduplikowany rekord urządzenia w portalu

Jeśli urządzenie nie zgłosi prawidłowo stanu współzarządzania witrynie programu Configuration Manager, w portalu mogą być widoczne dwa rekordy dla tego samego urządzenia. Stan współzarządzania urządzeniem możesz sprawdzić w kolumnie **Współzarządzane** dla urządzenia w konsoli programu Configuration Manager. Jeśli kolumna jest niewidoczna, możesz ją dodać, klikając prawym przyciskiem myszy dowolne nagłówki kolumn, a następnie wybierając ją z listy.

Kolumna Współzarządzane musi mieć wartość **Tak**. Jeśli wartość to **Nie**, otwórz aplet klienta Configuration Manager na urządzeniu klienckim i sprawdź wartość **Współzarządzanie** na karcie Ogólne.

- Jeśli wartość to **Włączone**, wskazuje to na problemy z komunikacją między klientem a punktem zarządzania. Sprawdź plik **CcmMessaging.log** na urządzeniu pod kątem potencjalnych problemów z łącznością.

- Jeśli wartość to **Wyłączone**, a urządzenie jest zarejestrowane w usłudze Intune, sprawdź plik **CoManagementHandler.log** na urządzeniu, aby upewnić się, że urządzenie otrzymało zasady współzarządzania.
