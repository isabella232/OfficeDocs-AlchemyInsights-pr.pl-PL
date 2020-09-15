---
title: Rozwiązano problem z buforem wydruku
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801851"
---
# <a name="print-spooler-issue-is-resolved"></a>Rozwiązano problem z buforem wydruku

Jeśli urządzenie zostało zaktualizowane w systemie operacyjnym Windows 10  **OS kompilacja 19041,329**, być może wystąpił problem polegający na tym, że niektóre drukarki nie są drukowane. Bufor wydruku może zgłosić błąd lub nieoczekiwane zamknięcie podczas próby wydrukowania, a żadne dane wyjściowe nie pochodzą z drukarki, której dotyczy problem. Ten problem został rozwiązany w systemie operacyjnym [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) **19041,331**.  

**Prowadzone badanie**

Plik usługi LSASS**Isass.exe**(Local Security Authority Subsystem Service) może się nie udać na niektóre urządzenia z komunikatem o błędzie "krytyczny proces systemowy, C:\WINDOWS\system32\Isass.exe, którego nie można znaleźć w kodzie statusu c0000008. Komputer musi być teraz ponownie uruchomiony.  **Firma Microsoft pracuje nad rozróżnieniem i będzie dostarczać aktualizację w nadchodzącej wersji.**

Aby uzyskać więcej informacji, zobacz  [znane problemy dotyczące systemu Windows 10 w wersji 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).