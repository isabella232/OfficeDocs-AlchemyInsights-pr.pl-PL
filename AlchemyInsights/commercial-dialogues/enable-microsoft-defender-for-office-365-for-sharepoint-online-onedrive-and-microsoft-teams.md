---
title: Włączanie Sejf załączników dla SharePoint Online, OneDrive i Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894473"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włączanie Sejf załączników dla SharePoint Online, OneDrive i Microsoft Teams

1. Używając poświadczeń administratora globalnego lub administratora zabezpieczeń, otwórz portal Microsoft 365 Defender w witrynie , a następnie przejdź do sekcji Zasady & reguły zagrożeń Sejf załączników w <https://security.microsoft.com>  \>  \>  **sekcji** Zasady.

   Aby przejść bezpośrednio do strony **załączników Sejf,** <https://security.microsoft.com/safeattachmentv2> użyj .

2. Na stronie **Sejf załączników** kliknij pozycję **Ustawienia globalne**.
3. W wyświetlonym wysuwu wybierz pozycję Włącz program Microsoft Defender dla systemu Office 365 dla systemu **SharePoint, OneDrive i** Microsoft Teams , a następnie wybierz pozycję **Zapisz**.

    > [!TIP]
    >
    > Wykonaj poniższe czynności, aby zwiększyć ochronę załączników Sejf załączników do SharePoint, OneDrive i Microsoft Teams:
    >
    > - Aby uniemożliwić użytkownikom pobieranie złośliwych plików, użyj wartości parametru `$true` *DisallowInfectedFileDownload* polecenia cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** w programie SharePoint Online PowerShell. Aby uzyskać więcej informacji, [zobacz Używanie programu PowerShell SharePoint Online,](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)aby uniemożliwić użytkownikom pobieranie złośliwych plików.
    > - [Tworzenie zasad alertów dla wykrytych plików](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Aby uzyskać więcej informacji, [zobacz Sejf załączniki Office 365 załączników](https://go.microsoft.com/fwlink/?linkid=2092041)do SharePoint, OneDrive i Microsoft Teams.
