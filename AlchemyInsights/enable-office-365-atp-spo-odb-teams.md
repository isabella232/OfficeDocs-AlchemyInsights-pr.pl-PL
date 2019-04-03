---
title: Włącz ATP Office 365 dla programu SharePoint, OneDrive i zespołów firmy Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031046"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Włącz pakietu Office 365 zaawansowaną ochronę przed zagrożeniami dla programu SharePoint w trybie Online, OneDrive i zespołów firmy Microsoft

1. Przejdź do https://protection.office.com i zaloguj się.
2. Wybierz opcję **Zarządzanie zagrożeniami** > **zasad** > **Bezpieczne załączniki**.
3. Wybierz opcję **Włącz ATP, SharePoint, usługi i zespoły pracowników firmy Microsoft**, a następnie kliknij przycisk **Zapisz**.
4. (Zalecane) Jako administratora globalnego lub administratora programu SharePoint w trybie Online należy uruchomić polecenie cmdlet [Set SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość true*.
5. (Zalecane) [Ustaw alerty](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dla wykrytych plików.

> [!NOTE]
> ATP będzie nto skanowania każdy pojedynczy plik programu SharePoint w trybie Online, OneDrive lub Teams firmy Microsoft. Pliki są skanowane asynchronicznie, poprzez proces, który używa udostępniania i Gość zdarzeń aktywności, wraz z heurystyki inteligentnego i sygnały zagrożenie do identyfikacji szkodliwych plików. Zobacz [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).