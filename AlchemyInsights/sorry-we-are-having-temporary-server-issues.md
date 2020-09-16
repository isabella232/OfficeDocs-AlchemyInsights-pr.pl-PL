---
title: Rozwiązywanie problemów z aplikacjami Microsoft 365 Przepraszamy, mamy komunikat o tymczasowych problemach z serwerem
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758255"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rozwiązywanie problemów z aplikacjami Microsoft 365 "Niestety, występują tymczasowe problemy z serwerami"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i ustawień serwera proxy, aby upewnić się, że nie blokuje dostępu do Internetu aplikacjom Microsoft 365. Zobacz [adresy URL i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Przejdź do **ekranu startowego**  >  **Run**, a następnie wpisz **Services. msc**. Upewnij się, że są uruchomione następujące usługi:
    - Automatyczne konfigurowanie urządzeń podłączonych do sieci
    - Usługa listy sieci
    - Rozpoznawanie lokalizacji w sieci
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli wystąpił problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc/scannow**

Po zakończeniu tego polecenia Uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można nawiązać połączenia z kontem. Podczas aktywowania spróbuj ponownie później](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).