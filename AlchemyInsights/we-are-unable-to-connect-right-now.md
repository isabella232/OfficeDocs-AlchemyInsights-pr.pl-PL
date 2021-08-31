---
title: Problem z aktywacją — nie można teraz nawiązać połączenia
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744605"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Naprawianie Microsoft 365 "Nie można teraz nawiązać połączenia"

Uwaga: Jeśli korzystasz ze starszej wersji programu Windows (na przykład Windows 7 z dodatkiem SP1, Windows Server 2008 R2), użyj łatwej poprawki, aby włączyć domyślną wartość TLS 1.2. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Aby uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślnych protokołów bezpiecznego w winieHTTP w programie Windows.

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu Microsoft 365 aplikacji. Zobacz [Adresy URL i zakresy adresów IP firmy Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Przejdź do  >  **startowego uruchamiania**, a następnie wpisz **services.msc.** Upewnij się, że wszystkie następujące usługi są uruchomione:
    - Automatyczne konfigurowanie urządzeń połączonych z siecią
    - Usługa listy sieciowej
    - Informacje o lokalizacji sieciowej
    - Windows Dziennik zdarzeń

Jeśli jedna z tych usług nie jest uruchomiona, spróbuj ją uruchomić. Jeśli masz problem z uruchomieniem usługi, uruchom następujące polecenie, otwierając wiersz polecenia z podwyższonym poziomem uprawnień:

**sfc /scannow**

Po zakończeniu tego polecenia uruchom ponownie komputer.

Aby uzyskać szczegółowe informacje, zobacz ["Niestety, nie można połączyć się z Twoim kontem. Spróbuj ponownie później" podczas aktywowania Office z Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)