---
title: Naprawianie błędu 0x8004de40 w OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133986"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Naprawianie błędu 0x8004de40 w OneDrive

Jeśli komunikat o błędzie 0x8004de40 z OneDrive:

- Uruchom ponownie dotyczy komputera podłączonego do domeny katalogu substancje czynne.
- Jeśli ponowny rozruch nie rozwiąże problemu, odłączyć i ponownie dołączyć urządzenie z Azure AD. 

**Uwaga**: należy zachować w sieci firmowej podczas wykonywania tych kroków. Nie wykonanie tych kroków, gdy nie są w stanie nawiązać połączenia sieci firmowej infrastruktury (na przykład podczas podróży). 

- Otwórz wiersz polecenia z podwyższonym poziomem uprawnień. 
- Aby otworzyć wiersz polecenia, kliknij przycisk - **Start**, kliknij prawym przyciskiem myszy **Wiersz polecenia**, a następnie kliknij **Uruchom jako administrator**.
- *Dsregcmd /leave* i naciśnij klawisz **Enter**.
- Po zakończeniu, *wpisz/JOIN dsregcmd* i naciśnij klawisz **Enter**.
- Po zakończeniu zamknij okno wiersza polecenia.
- Uruchom ponownie komputer i zaloguj się do OneDrive.