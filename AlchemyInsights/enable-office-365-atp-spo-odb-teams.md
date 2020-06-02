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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506928"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włączanie zaawansowanej ochrony przed zagrożeniami usługi Office 365 dla usługi SharePoint Online, OneDrive i Microsoft Teams

1. Przejdź do https://protection.office.com i zaloguj się.
2. Wybierz **Threat management**pozycję Bezpieczne  >  **Policy**  >  **załączniki zasad zarządzania zagrożeniami**.
3. Wybierz **pozycję Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.
4. (Zalecane) Jako administrator globalny lub administrator usługi SharePoint Online uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **Nieustawianie InfectedFileDownload** ustawionym na *wartość true*.
5. (Zalecane) [Skonfiguruj alerty](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczące wykrytych plików.

> [!NOTE]
> Narzędzie ATP będzie skanować każdy plik w usłudze SharePoint Online, OneDrive lub usłudze Microsoft Teams. Pliki są skanowane asynchronicznie, za pośrednictwem procesu, który używa udostępniania i zdarzeń aktywności gościa, wraz z inteligentną heurystyką i sygnałami zagrożeń do identyfikacji złośliwych plików. Zobacz [ATP dla programu SharePoint, OneDrive i Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).