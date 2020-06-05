---
title: Problem z aktywacją - Nie możemy teraz połączyć się
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581885"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Naprawianie komunikatu "Nie możemy teraz połączyć się z aplikacjami usługi Microsoft 365"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują dostępu do Internetu do aplikacji usługi Microsoft 365. Zobacz [adresy URL firmy Microsoft i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Przejdź do **ekranu**  >  **Uruchom**, a następnie wpisz **plik services.msc**. Upewnij się, że wszystkie następujące usługi są uruchomione:
    - Automatyczna konfiguracja urządzeń podłączonych do sieci
    - Usługa listy sieci
    - Rozpoznawanie lokalizacji sieciowej
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc /scannow**

Po zakończeniu tego polecenia uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy połączyć się z Twoim kontem. Spróbuj ponownie później" błąd po przyśpiesze office z usługi Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).