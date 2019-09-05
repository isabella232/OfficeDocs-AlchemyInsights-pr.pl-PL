---
title: Napraw błąd 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755858"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Napraw błąd 0x8004de40 w usłudze OneDrive

Jeśli zostanie wyświetlony błąd 0x8004de40 z OneDrive:

- Uruchom ponownie komputer, którego dotyczy problem, po podłączeniu do domeny katalogu Acitve.
- Jeśli ponowne uruchomienie nie rozwiąże problemu, odłączenie i ponowne dołączenie urządzenia z usługi Azure AD. 

**Uwaga**: podczas wykonywania tych czynności powinieneś być w sieci firmowej. Nie wykonuj tych czynności, gdy nie możesz nawiązać połączenia z infrastrukturą firmową (na przykład podczas podróży). 

- Otwórz wiersz polecenia z podwyższonym poziomem uprawnień. 
- Aby otworzyć wiersz polecenia z podwyższonym poziomem uprawnień, kliknij przycisk **Start**, kliknij prawym przyciskiem myszy **wiersz polecenia**, a następnie kliknij polecenie **Uruchom jako administrator**.
- Wpisz *polecenie dsregcmd/Leave* i naciśnij **Enter**.
- Po zakończeniu wpisz *polecenie dsregcmd/Join* i naciśnij **Enter**.
- Po zakończeniu Zamknij wiersz polecenia.
- Uruchom ponownie komputer i zaloguj się do usługi OneDrive.