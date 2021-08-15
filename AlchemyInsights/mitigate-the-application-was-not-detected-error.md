---
title: Korygowanie błędu „Aplikacja nie została wykryta”
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
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026124"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Korygowanie błędu „Aplikacja nie została wykryta”

Błąd instalacji aplikacji „Aplikacja nie została wykryta po pomyślnym zakończeniu instalacji” zgłaszany przez usługę Intune może wystąpić na wszystkich głównych platformach systemu operacyjnego (Windows, iOS i Android).

Najczęstsze scenariusze, w których jest generowany ten błąd, są następujące:

- Aplikacja została zaktualizowana poza usługą Intune (ze sklepu z aplikacjami innego producenta) po wdrożeniu początkowym. Na przykład niektóre aplikacje, takie jak Google Chrome, mogą wykonywać aktualizacje automatyczne.
- Użytkownik odinstalował aplikację po początkowej instalacji.

Aby rozwiązać ten problem, najpierw sprawdź dotknięte problemem urządzenia w celu ustalenia, z jakim scenariuszem tego błędu masz do czynienia.

- Jeśli aplikacja została zaktualizowana poza usługą Intune, dla wdrożenia aplikacji można ustawić ignorowanie wersji aplikacji. W tym celu w obszarze **Konfiguracja aplikacji > Informacje o aplikacji** ustaw dla opcji **Ignoruj wersję aplikacji** wartość **Tak**.
- W przypadku kierowania do klienta być może warto wdrożyć aplikację jako „wymaganą”, aby upewnić się, że zostanie wdrożona najnowsza wersja.
- Natomiast na platformie iOS możliwe jest używanie funkcji **automatycznej aktualizacji** skojarzonej z programem zakupów grupowych Apple Volume Purchase Program, który można skonfigurować tak, aby automatycznie aktualizować aplikacje do nowych wersji po ich udostępnieniu.

Aby uzyskać więcej informacji na temat rozwiązywania problemów z instalacją aplikacji, zobacz [Rozwiązywanie problemów z instalacją aplikacji](https://docs.microsoft.com/intune/troubleshoot-app-install).
