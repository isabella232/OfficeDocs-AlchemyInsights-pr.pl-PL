---
title: ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715571"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams

Wykonaj poniższe czynności, aby włączyć zaawansowaną ochronę przed zagrożeniami:

1. Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się przy użyciu konta administratora globalnego lub administratora zabezpieczeń.

2. W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **zasady** \> **bezpieczne załączniki**.

3. Wybierz pozycję **Włącz ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams**.

4. [Utwórz zasady alertów aktywności](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , aby otrzymywać powiadomienia o wykryciu złośliwych plików.

Aby uzyskać pełne instrukcje, zapoznaj się z tym [tematem](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Uwaga**: według projektu ATP nie skanuje każdego pojedynczego pliku w usłudze SharePoint Online, OneDrive dla firm lub aplikacji Microsoft Teams. Pliki są skanowane asynchronicznie przez proces umożliwiający identyfikowanie złośliwych plików za pomocą procesu udostępniania, aktywności gościa i sygnałów dotyczących zagrożeń. Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
