---
title: Naprawianie błędu 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745140"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Naprawianie błędu 0x8004de40 w usłudze OneDrive

Jeśli podczas korzystania z usługi OneDrive Wystąpił błąd 0x8004de40:

- Uruchom ponownie komputer, którego dotyczy problem, gdy połączysz się z domeną usługi Acitve.
- Jeśli ponowne uruchomienie komputera nie rozwiązało problemu, odłączanie i ponowne dołączanie do urządzenia z usługi Azure AD. 

**Uwaga**: w celu wykonania tych czynności należy korzystać z sieci firmowej. Nie wykonuj tych czynności, gdy nie możesz połączyć się z infrastrukturą firmową (na przykład podczas podróży). 

- Otwórz wiersz polecenia z podwyższonym poziomem uprawnień. 
- Aby otworzyć wiersz polecenia z podwyższonym poziomem uprawnień, kliknij przycisk **Start**, kliknij prawym przyciskiem myszy pozycję **wiersz polecenia**, a następnie kliknij polecenie **Uruchom jako administrator**.
- Wpisz *dsregcmd/Leave* i naciśnij klawisz **Enter**.
- Po zakończeniu wpisz *dsregcmd/Join* i naciśnij klawisz **Enter**.
- Po zakończeniu Zamknij wiersz polecenia.
- Uruchom ponownie komputer i zaloguj się do usługi OneDrive.