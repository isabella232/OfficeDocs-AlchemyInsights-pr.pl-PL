---
title: 932 AADConnect uaktualniania
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778751"
---
# <a name="upgrade-azure-ad-connect"></a>Podłącz uaktualnienia Azure AD

Domyślnie automatyczne uaktualnienie jest włączona dla Azure AD Connect, które pomaga zapewnić, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia automatycznego uaktualniania, należy użyć polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie AD PowerShell Azure. Polecenia cmdlet zwróci się jedną z następujących wartości: 
  
- **Włączone**: automatyczne uaktualnienie jest włączona. 
    
- **Wyłączone**: automatyczne uaktualnienie jest wyłączane. 
    
- **Zawieszone**: system nie jest już uprawniony do otrzymania automatycznych uaktualnień. Nie można skonfigurować tej wartości; jest on ustawiony przez system. 
    
Aby uzyskać więcej informacji zobacz temat [automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Aby pobrać najnowszą wersję programu Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

