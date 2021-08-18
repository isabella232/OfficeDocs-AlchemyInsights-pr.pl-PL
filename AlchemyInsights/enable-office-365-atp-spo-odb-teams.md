---
title: Włączanie Office 365 ATP dla SharePoint, OneDrive i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332169"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włączanie usługi Microsoft Defender dla Office 365 dla SharePoint Online, OneDrive i Microsoft Teams

1. Przejdź do https://protection.office.com i zaloguj się.
2. Wybierz **pozycję Zasady zarządzania**  >  **zagrożeniami**  >  **Sejf załączników.**
3. Wybierz **pozycję Włącz defender dla Office 365 dla SharePoint, OneDrive i Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.
4. (Zalecane) Jako administrator globalny lub administrator usługi SharePoint Online uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość true.*
5. (Zalecane) [Konfigurowanie alertów dotyczących](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) wykrytych plików.

**Uwaga:** Program Microsoft Defender dla systemu Office 365 nie skanuje wszystkich plików w aplikacjach SharePoint Online, OneDrive i Microsoft Teams. Pliki są skanowane asynchronicznie w ramach procesu, który używa zdarzeń udostępniania i aktywności gościa, a także inteligentnych heuristics i sygnałów zagrożeń do identyfikowania złośliwych plików. Zobacz [Program Microsoft Defender Office 365, SharePoint, OneDrive i Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
