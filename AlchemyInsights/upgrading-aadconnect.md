---
title: 932 Uaktualnianie programu AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104822"
---
# <a name="upgrade-azure-ad-connect"></a>Uaktualnianie usługi Azure AD Połączenie

Domyślnie automatyczne uaktualnianie jest włączone dla usługi Azure AD Połączenie, co pomaga upewnić się, że używasz najnowszej wersji. Aby zweryfikować ustawienia automatycznego uaktualniania, użyj polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie PowerShell usługi Azure AD. Polecenie cmdlet zwróci jedną z następujących wartości:

- **Włączone:** Automatyczne uaktualnianie jest włączone.

- **Wyłączone:** Automatyczne uaktualnianie jest wyłączone.

- **Wstrzymane:** System nie jest już uprawniony do otrzymywania uaktualnień automatycznych. Tej wartości nie można skonfigurować; jest ustawiana przez system.

Aby uzyskać więcej informacji, zobacz [Automatyczne uaktualnianie.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Aby pobrać najnowszą wersję narzędzia Azure AD Połączenie, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) strony .
