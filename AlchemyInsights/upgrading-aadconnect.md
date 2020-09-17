---
title: 932 uaktualnianie AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806049"
---
# <a name="upgrade-azure-ad-connect"></a>Uaktualnij usługę Azure AD Connect

Domyślnie automatyczne uaktualnienie jest włączone dla usługi Azure AD Connect, co zapewnia, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia uaktualnienia automatycznego, użyj polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie Azure AD PowerShell. Polecenie cmdlet zwróci dowolną z następujących wartości:

- **Włączone**: automatyczne uaktualnianie jest włączone.

- **Wyłączone**: automatyczne uaktualnienie jest wyłączone.

- **Zawieszone**: system nie kwalifikuje się już do otrzymywania automatycznych uaktualnień. Tej wartości nie można skonfigurować; jest ona ustawiana przez system.

Aby uzyskać więcej informacji, zobacz [automatyczne uaktualnianie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Aby pobrać najnowszą wersję usługi Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
