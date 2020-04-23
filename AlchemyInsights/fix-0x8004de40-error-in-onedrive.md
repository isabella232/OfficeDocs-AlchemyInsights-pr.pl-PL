---
title: Napraw błąd 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716038"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Napraw błąd 0x8004de40 w usłudze OneDrive

Jeśli w usłudze OneDrive zostanie wyświetlony błąd 0x8004de40:

- Uruchom ponownie komputer, którego dotyczy problem, po podłączeniu do domeny katalogu Acitve.
- Jeśli ponowne uruchomienie nie rozwiąże problemu, odłącz urządzenie i dołącz ponownie do urządzenia z usługi Azure AD. 

**Uwaga:** Podczas wykonywania tych czynności powinien znajdować się w sieci firmowej. Nie wykonuj tych czynności, gdy nie możesz połączyć się z infrastrukturą firmową (na przykład podczas podróży). 

- Otwórz wiersz polecenia z podwyższonym poziomem uprawnień. 
- Aby otworzyć wiersz polecenia z podwyższonem poziomem uprawnień, kliknij przycisk - **Start**, kliknij prawym przyciskiem myszy **wiersz polecenia**, a następnie kliknij polecenie Uruchom **jako administrator**.
- Wpisz *dsregcmd /leave* i naciśnij **klawisz Enter**.
- Po zakończeniu wpisz *dsregcmd /join* i naciśnij **klawisz Enter**.
- Po zakończeniu zamknij wiersz polecenia.
- Uruchom ponownie komputer i zaloguj się do usługi OneDrive.