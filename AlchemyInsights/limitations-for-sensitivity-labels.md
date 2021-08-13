---
title: Ograniczenia dotyczące etykiet wrażliwości Office plików w SharePoint i OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813162"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Ograniczenia dotyczące etykiet wrażliwości Office plików w SharePoint i OneDrive

Podczas włączania etykiet wrażliwości Office plików w SharePoint i OneDrive należy pamiętać o wymaganiach i ograniczeniach, takich jak:

- SharePoint i OneDrive nie mogą przetwarzać niektórych plików oznaczonych i zaszyfrowanych z aplikacji klasycznych pakietu Office, gdy te pliki zawierają dane usługi PowerQuery, dane przechowywane przez dodatki niestandardowe lub niestandardowe części XML.
- SharePoint i OneDrive etykiet wrażliwości nie są automatycznie stosowane do istniejących plików już zaszyfrowanych przy użyciu etykiet usługi Azure Information Protection (AIP). Aby zastosować etykiety wrażliwości do zaszyfrowanych plików: 
    - Upewnij się, że etykiety AIP zostały zmigrowane i opublikowane w Centrum Microsoft 365 zgodności.
    - Pobierz pliki oznaczone etykietą, a następnie przekaż je do ich SharePoint lub OneDrive lokalizacji.
- W przypadku zaszyfrowanych dokumentów drukowanie nie jest obsługiwane.

Aby uzyskać dodatkowe informacje na temat ograniczeń, zobacz Włączanie etykiet wrażliwości Office plików w SharePoint [i OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
