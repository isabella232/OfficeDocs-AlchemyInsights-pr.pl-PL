---
title: Włącz usługę Office 365 ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709917"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>365 Włączanie zaawansowanej ochrony przed zagrożeniami dla usługi SharePoint Online, OneDrive i Microsoft Teams

1. Przejdź do https://protection.office.com i zaloguj się.
2. Wybieranie **Threat management**  >  **Policy**  >  **bezpiecznych załączników**zasad zarządzania zagrożeniami.
3. Wybierz pozycję **Włącz ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.
4. Zalecon Jako Administrator globalny lub administrator usługi SharePoint Online Uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** o wartości *true*.
5. Zalecon [Konfigurowanie alertów](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczących wykrytych plików.

> [!NOTE]
> ATP usunie skanowanie każdego pojedynczego pliku w usłudze SharePoint Online, OneDrive lub Microsoft Teams. Pliki są skanowane asynchronicznie za pomocą procesu, w którym są używane zdarzenia dotyczące udostępniania i aktywności gościa, a także inteligentne heurystyka i sygnały zagrożeń w celu zidentyfikowania złośliwych plików. Zobacz [ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).