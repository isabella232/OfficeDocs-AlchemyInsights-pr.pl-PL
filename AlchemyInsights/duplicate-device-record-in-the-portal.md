---
title: Zduplikowany rekord urządzenia w portalu
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
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004164"
---
# <a name="duplicate-device-record-in-the-portal"></a>Zduplikowany rekord urządzenia w portalu

Jeśli urządzenie nie zgłosi prawidłowo stanu współzarządzania witrynie programu Configuration Manager, w portalu mogą być widoczne dwa rekordy dla tego samego urządzenia. Stan współzarządzania urządzeniem możesz sprawdzić w kolumnie **Współzarządzane** dla urządzenia w konsoli programu Configuration Manager. Jeśli kolumna jest niewidoczna, możesz ją dodać, klikając prawym przyciskiem myszy dowolne nagłówki kolumn, a następnie wybierając ją z listy.

Kolumna Współzarządzane musi mieć wartość **Tak**. Jeśli wartość to **Nie**, otwórz aplet klienta Configuration Manager na urządzeniu klienckim i sprawdź wartość **Współzarządzanie** na karcie Ogólne.

- Jeśli wartość to **Włączone**, wskazuje to na problemy z komunikacją między klientem a punktem zarządzania. Sprawdź plik **CcmMessaging.log** na urządzeniu pod kątem potencjalnych problemów z łącznością.

- Jeśli wartość to **Wyłączone**, a urządzenie jest zarejestrowane w usłudze Intune, sprawdź plik **CoManagementHandler.log** na urządzeniu, aby upewnić się, że urządzenie otrzymało zasady współzarządzania.
