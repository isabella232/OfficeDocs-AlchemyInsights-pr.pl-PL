---
title: Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 Niestety, mamy komunikat o tymczasowych problemach z serwerem
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835281"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Naprawianie aplikacji platformy Microsoft 365 Komunikat "Niestety, mamy problemy z serwerem tymczasowych"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu do aplikacji platformy Microsoft 365. Zobacz [Adresy URL i zakresy adresów IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Przejdź do  >  **startowego uruchamiania**, a następnie wpisz **services.msc.** Upewnij się, że wszystkie następujące usługi są uruchomione:
    - Automatyczne konfigurowanie urządzeń połączonych z siecią
    - Usługa listy sieciowej
    - Informacje o lokalizacji sieciowej
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc /scannow**

Po zakończeniu tego polecenia uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można połączyć się z Twoim kontem. Spróbuj ponownie później" podczas aktywowania](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).