---
title: Naprawianie 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649758"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Naprawianie 0x8004de40 w usłudze OneDrive

Jeśli używasz systemu Windows 7 i otrzymujesz ten błąd, zaktualizuj go, aby włączyć [protokoły TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślne protokoły bezpiecznego w systemie WinHTTP w systemie Windows.

Jeśli używasz systemu Windows 10 i jest wyświetlany komunikat o błędzie 0x8004de40 usługi OneDrive:

- Uruchom ponownie komputer, którego dotyczy problem, podczas połączenia z domeną katalogu Acitve.
- Jeśli ponowne uruchomienie nie rozwiąże problemu, rozłącz i ponownie dołącz do urządzenia z usługi Azure AD. 

**Uwaga:** podczas wykonywania tych czynności powinno się być w sieci firmowej. Nie wykonuj tych czynności, gdy nie masz połączenia z infrastrukturą firmową (na przykład w podróży). 

1. Otwórz wiersz polecenia z podwyższonym poziomem uprawnień, wybierając **przycisk Start**, kliknij prawym przyciskiem myszy pozycję Wiersz **polecenia**, a następnie wybierz pozycję Uruchom **jako administrator.**

1. Wpisz *dsregcmd /leave i* naciśnij klawisz **Enter.**

1. Po zakończeniu wpisz *dsregcmd /join* i naciśnij klawisz **Enter.**

1. Po zakończeniu zamknij wiersz polecenia.

1. Uruchom ponownie komputer i zaloguj się do usługi OneDrive.