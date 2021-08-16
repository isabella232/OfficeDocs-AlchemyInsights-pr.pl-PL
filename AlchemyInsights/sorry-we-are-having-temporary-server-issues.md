---
title: Naprawianie Microsoft 365 niestety, mamy komunikat o tymczasowych problemach z serwerem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021606"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Naprawianie Microsoft 365 "Niestety, mamy problemy z serwerem tymczasowych"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu Microsoft 365 aplikacji. Zobacz [Adresy URL i zakresy adresów IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Przejdź do  >  **startowego uruchamiania**, a następnie wpisz **services.msc.** Upewnij się, że wszystkie następujące usługi są uruchomione:
    - Automatyczne konfigurowanie urządzeń połączonych z siecią
    - Usługa listy sieciowej
    - Informacje o lokalizacji sieciowej
    - Windows Dziennik zdarzeń

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc /scannow**

Po zakończeniu tego polecenia uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można połączyć się z Twoim kontem. Spróbuj ponownie później" podczas aktywowania](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).