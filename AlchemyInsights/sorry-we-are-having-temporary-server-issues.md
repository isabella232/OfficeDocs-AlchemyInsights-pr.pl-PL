---
title: Naprawianie aplikacji pakietu Office Przepraszamy, mamy tymczasowy problem z serwerem wiadomości
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628000"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Naprawianie aplikacji pakietu Office "Przepraszamy, mamy tymczasowe problemy z serwerem" wiadomość

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory sieciowej, oprogramowania antywirusowego i serwera proxy, aby potwierdzić, że nie blokują dostępu do Internetu aplikacjom pakietu Office. Zobacz [adresy url 365 pakietu Office i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Przejdź do **Start** > **Run**, a następnie wpisz **Services. msc**. Upewnij się, że są uruchomione następujące usługi:
    - Automatyczna konfiguracja urządzeń podłączonych do sieci
    - Usługa listy sieci
    - Rozpoznawanie lokalizacji w sieci
    - Dziennik zdarzeń systemu Windows

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc/scannow**

Po zakończeniu tego polecenia Uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Przepraszamy, nie możemy nawiązać połączenia z Twoim kontem. Spróbuj ponownie później "błąd podczas aktywowania pakietu Office z pakietu Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).