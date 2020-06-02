---
title: ATP dla programu SharePoint, OneDrive i Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508422"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP dla programu SharePoint, OneDrive i Microsoft Teams

Wykonaj następujące kroki, aby włączyć zaawansowaną ochronę przed zagrożeniami:

1. Przejdź do [https://protection.office.com](https://protection.office.com) konta administratora globalnego lub administratora zabezpieczeń i zaloguj się.

2. W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Policy** \> **Załączniki bezpieczne dla zasad**.

3. Wybierz **pozycję Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams**.

4. [Utwórz zasady alertów aktywności,](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) aby otrzymywać powiadomienia, gdy wykryjemy złośliwe pliki.

Aby uzyskać pełne instrukcje, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Uwaga:** Zgodnie z projektem narzędzie ATP nie skanuje każdego pliku w usłudze SharePoint Online, usłudze OneDrive dla Firm ani w usłudze Microsoft Teams. Pliki są skanowane asynchronicznie przez proces, który używa aktywności udostępniania, aktywności gościa i sygnałów zagrożeń do identyfikowania złośliwych plików. Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
