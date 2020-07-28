---
title: Sterowanie automatycznymi aktualizacjami aplikacji pakietu Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439920"
---
# <a name="control-automatic-updates-for-office-apps"></a>Sterowanie automatycznymi aktualizacjami aplikacji pakietu Office

Domyślnie aktualizacje aplikacji pakietu Office są pobierane automatycznie i stosowane w tle bez interwencji użytkownika. Administratorzy mogą jednak kontrolować sposób stosowania aktualizacji przy użyciu ustawień aktualizacji pakietu Office. Ustawienia aktualizacji umożliwiają administratorom włączanie lub wyłączanie aktualizacji automatycznych, pokazywanie lub ukrywanie przycisku **Aktualizuj teraz** w pakiecie Office, ustawianie terminów aktualizacji i inne. Aby uzyskać szczegółowe informacje, zobacz:

- [Konfigurowanie ustawień aktualizacji pakietu Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatyczne aktualizowanie pakietu Office nie jest włączone](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiowanie sposobu aktualizowania pakietu Office po zainstalowaniu](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Aby przejrzeć istniejące ustawienia aktualizacji zastosowane do komputera klienckiego, wykonaj następujące kroki:

1. Otwórz Edytor rejestru, przechodząc do **ekranu**  >  **startowego**  >  **regedit**.
2. Przełącz się do następującej lokalizacji i przejrzyj ustawienia aktualizacji pakietu Office:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Konfiguracja

**Uwaga**  Jeśli jest ustawiony klucz OfficeMgmtCOM, w **Office**  >  **Account**  >  **aktualizacjech pakietu**Office może zostać wyświetlony komunikat "Aktualizacje są zarządzane przez administratora systemu". Aby uzyskać więcej informacji, zobacz [Zarządzanie aktualizacjami aplikacji usługi Microsoft 365 za pomocą programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  