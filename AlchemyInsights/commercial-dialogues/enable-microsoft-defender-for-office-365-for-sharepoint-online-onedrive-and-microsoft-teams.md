---
title: Włączanie usługi Microsoft Defender dla Office 365 dla SharePoint Online, OneDrive i Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058876"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włączanie usługi Microsoft Defender dla Office 365 dla SharePoint Online, OneDrive i Microsoft Teams

1. Korzystając z poświadczeń administratora globalnego lub administratora zabezpieczeń, zaloguj się do centrum Office 365 [zabezpieczeń i zgodności.](https://protection.office.com/)
2. Wybierz **pozycję Zarządzanie zagrożeniami** w lewym okienku, a następnie wybierz **pozycję**  >  [Sejf załączników](https://protection.office.com/safeattachment).
3. Wybierz **pozycję Włącz program Microsoft Defender dla Office 365 dla SharePoint, OneDrive i Microsoft Teams**, a następnie wybierz pozycję **Zapisz**.
    > [!TIP]
    >
    > - Jako administrator globalny lub administrator usługi SharePoint Online uruchom następujące polecenie cmdlet programu PowerShell z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurowanie alertów dotyczących wykrytych plików](https://go.microsoft.com/fwlink/?linkid=2092110)

Aby uzyskać więcej informacji, zobacz [Program Microsoft Defender for Office 365 for SharePoint, OneDrive and Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
