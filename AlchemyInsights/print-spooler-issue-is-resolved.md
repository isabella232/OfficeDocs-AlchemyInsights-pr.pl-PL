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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911348"
---
# <a name="print-spooler-issue-is-resolved"></a>Rozwiązano problem z buforem wydruku

Jeśli urządzenie zostało zaktualizowane za pomocą Windows 10 systemu operacyjnego **19041.329,** możesz zaobserwować problem z drukowaniem niektórych drukarek.   Bufor wydruku może zgłosić błąd lub zamknąć się nieoczekiwanie podczas próby wydrukowania, a dane wyjściowe nie pochodzą z drukarki, na która wpływa. Ten problem został rozwiązany w kompilacji systemu operacyjnego **19041.331**, [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Bieżące badanie**

Plik usługi podsystemu Local Security Authority Service (LSASS)**(Isass.exe)** może się nie powieść na niektórych urządzeniach z komunikatem o błędzie "Krytyczny proces systemowy, C:\WINDOWS\system32\Isass.exe, nie powiodło się z kodem stanu c0000008. Komputer musi zostać ponownie uruchomiony".  **Firma Microsoft pracuje nad jego rozwiązaniem i udostępni aktualizację w przyszłej wersji.**

Aby uzyskać więcej informacji, zapoznaj się z Windows 10 znane problemy z [wersją 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)