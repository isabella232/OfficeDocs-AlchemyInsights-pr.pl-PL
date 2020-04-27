---
title: Korygowanie błędu „Aplikacja nie została wykryta”
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810493"
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
