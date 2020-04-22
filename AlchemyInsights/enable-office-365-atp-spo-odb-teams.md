---
title: Włączanie usługi Office 365 ATP dla programu SharePoint, usługi OneDrive i usługi Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703436"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włączanie zaawansowanej ochrony przed zagrożeniami usługi Office 365 dla usługi SharePoint Online, OneDrive i Microsoft Teams

1. Przejdź https://protection.office.com do i zaloguj się.
2. Wybierz pozycję Bezpieczne załączniki**zasad** >  **zarządzania zagrożeniami** > .**Safe Attachments**
3. Wybierz **pozycję Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.
4. (Zalecane) Jako administrator globalny lub administrator usługi SharePoint Online uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **Nieustawianie InfectedFileDownload** ustawionym na *wartość true*.
5. (Zalecane) [Skonfiguruj alerty](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczące wykrytych plików.

> [!NOTE]
> Narzędzie ATP będzie skanować każdy plik w usłudze SharePoint Online, OneDrive lub usłudze Microsoft Teams. Pliki są skanowane asynchronicznie, za pośrednictwem procesu, który używa udostępniania i zdarzeń aktywności gościa, wraz z inteligentną heurystyką i sygnałami zagrożeń do identyfikacji złośliwych plików. Zobacz [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).