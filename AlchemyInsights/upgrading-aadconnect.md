---
title: 932 AADConnect uaktualniania
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757301"
---
# <a name="upgrade-azure-ad-connect"></a>Podłącz uaktualnienia Azure AD

Domyślnie automatyczne uaktualnienie jest włączona dla Azure AD Connect, które pomaga zapewnić, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia automatycznego uaktualniania, należy użyć polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie AD PowerShell Azure. Polecenia cmdlet zwróci się jedną z następujących wartości: 

- **Włączone**: automatyczne uaktualnienie jest włączona.

- **Wyłączone**: automatyczne uaktualnienie jest wyłączane.

- **Zawieszone**: system nie jest już uprawniony do otrzymania automatycznych uaktualnień. Nie można skonfigurować tej wartości; jest on ustawiony przez system. 

Aby uzyskać więcej informacji zobacz temat [automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Aby pobrać najnowszą wersję programu Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
