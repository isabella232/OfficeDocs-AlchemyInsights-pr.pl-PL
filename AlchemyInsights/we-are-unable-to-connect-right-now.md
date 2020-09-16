---
title: Problem z aktywacją — obecnie nie możemy nawiązać połączenia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725993"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Rozwiązywanie problemów z aplikacjami Microsoft 365 "komunikat nie można teraz połączyć"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i ustawień serwera proxy, aby upewnić się, że nie blokuje dostępu do Internetu aplikacjom Microsoft 365. Zobacz [adresy URL i zakresy adresów IP firmy Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Przejdź do **ekranu startowego**  >  **Run**, a następnie wpisz **Services. msc**. Upewnij się, że są uruchomione następujące usługi:
    - Automatyczne konfigurowanie urządzeń podłączonych do sieci
    - Usługa listy sieci
    - Rozpoznawanie lokalizacji w sieci
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli wystąpił problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc/scannow**

Po zakończeniu tego polecenia Uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później "błąd podczas aktywowania pakietu Office z usługi Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).