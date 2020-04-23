---
title: 932 Modernizacja AAdConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766503"
---
# <a name="upgrade-azure-ad-connect"></a>Uaktualnianie usługi Azure AD Connect

Domyślnie automatyczne uaktualnianie jest włączone dla usługi Azure AD Connect, co pomaga upewnić się, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia automatycznego uaktualniania, użyj polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie Azure AD PowerShell. Polecenie cmdlet zwróci jedną z następujących wartości:

- **Włączone:** Automatyczne uaktualnianie jest włączone.

- **Wyłączone**: Automatyczne uaktualnianie jest wyłączone.

- **Zawieszone**: System nie kwalifikuje się już do automatycznych uaktualnień. Nie można skonfigurować tej wartości; jest ustawiony przez system.

Aby uzyskać więcej informacji, zobacz [Automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Aby pobrać najnowszą wersję usługi Azure [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)AD Connect, przejdź do .
