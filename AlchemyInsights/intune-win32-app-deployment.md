---
title: Wdrożenie aplikacji Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461875"
---
# <a name="intune-win32-app-deployment"></a>Wdrożenie aplikacji Intune Win32

Usługa Microsoft Intune umożliwia aplikacjom systemu Win32, między innymi MSI i bez ograniczeń. EXE, który ma zostać wdrożony na urządzeniach z systemem Windows 10. Do korzystania z tego mechanizmu wdrażania jest wymagane rozszerzenie zarządzania usługą Intune (IME) na urządzeniu docelowym. Edytor IME zostanie zainstalowany automatycznie w wyniku przekierowania skryptu programu PowerShell lub wdrożenia aplikacji systemu Win32 do użytkownika/urządzenia.

Ponadto są dostępne wymagania wstępne, które muszą być spełnione w celu wdrożenia aplikacji Win32 zawierających następujące funkcje:

- Obsługiwane platformy: Windows 10 w wersji 1607 lub nowszej (wersje Enterprise, Pro i Education).
- Obsługiwana architektura: x86 i x64.
- Zarządzanie urządzeniami: dołączona i automatycznie zarejestrowana w usłudze AAD (w tym przyłączone domeny hybrydowe i zasady grupy są automatycznie rejestrowane).
- Format pakietu aplikacji:. **intunewin**  plik przygotowany za pomocą [narzędzia Microsoft Win32 Content przygotowywanie](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Określone
    - Maksymalny rozmiar: 8 GB.
    - Nieobsługiwana architektura: poręcze.

Przejrzyj dokument "[Dodawanie, przypisywanie i monitorowanie aplikacji systemu Win32 w usłudze Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)", aby uzyskać informacje dotyczące tych kroków.

Szczegółowe informacje dotyczące rozwiązywania problemów z wdrażaniem aplikacji w systemie Windows, w tym aplikacje systemu Win32, można przejrzeć w następujących dokumentach

- [Rozwiązywanie problemów z instalacją aplikacji](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Rozwiązywanie problemów z aplikacjami Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)