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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814526"
---
# <a name="duplicate-device-record-in-the-portal"></a>Zduplikowany rekord urządzenia w portalu

Jeśli urządzenie nie zgłosi prawidłowo stanu współzarządzania witrynie programu Configuration Manager, w portalu mogą być widoczne dwa rekordy dla tego samego urządzenia. Stan współzarządzania urządzeniem możesz sprawdzić w kolumnie **Współzarządzane** dla urządzenia w konsoli programu Configuration Manager. Jeśli kolumna jest niewidoczna, możesz ją dodać, klikając prawym przyciskiem myszy dowolne nagłówki kolumn, a następnie wybierając ją z listy.

Kolumna Współzarządzane musi mieć wartość **Tak**. Jeśli wartość to **Nie**, otwórz aplet klienta Configuration Manager na urządzeniu klienckim i sprawdź wartość **Współzarządzanie** na karcie Ogólne.

- Jeśli wartość to **Włączone**, wskazuje to na problemy z komunikacją między klientem a punktem zarządzania. Sprawdź plik **CcmMessaging.log** na urządzeniu pod kątem potencjalnych problemów z łącznością.

- Jeśli wartość to **Wyłączone**, a urządzenie jest zarejestrowane w usłudze Intune, sprawdź plik **CoManagementHandler.log** na urządzeniu, aby upewnić się, że urządzenie otrzymało zasady współzarządzania.
