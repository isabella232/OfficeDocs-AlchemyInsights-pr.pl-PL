---
title: Naprawianie aplikacji pakietu Office Niestety, mamy komunikat o tymczasowych problemach z serwerem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764127"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rozwiązywanie komunikatu "Przepraszamy, mamy tymczasowe problemy z serwerem"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują dostępu do Internetu w aplikacjach pakietu Office. Zobacz [adresy URL i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Przejdź do **ekranu** > **Uruchom**, a następnie wpisz **plik services.msc**. Upewnij się, że wszystkie następujące usługi są uruchomione:
    - Automatyczna konfiguracja urządzeń podłączonych do sieci
    - Usługa listy sieci
    - Rozpoznawanie lokalizacji sieciowej
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc /scannow**

Po zakończeniu tego polecenia uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy połączyć się z Twoim kontem. Spróbuj ponownie później" błąd po aktywacji](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).