---
title: 932 AADConnect uaktualniania
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304716"
---
# <a name="upgrade-azure-ad-connect"></a>Podłącz uaktualnienia Azure AD

Domyślnie automatyczne uaktualnienie jest włączona dla Azure AD Connect, które pomaga zapewnić, że korzystasz z najnowszej wersji. Aby sprawdzić ustawienia automatycznego uaktualniania, należy użyć polecenia cmdlet **Get-ADSyncAutoUpgrade** w programie AD PowerShell Azure. Polecenia cmdlet zwróci się jedną z następujących wartości: 
  
- **Włączone**: automatyczne uaktualnienie jest włączona. 
    
- **Wyłączone**: automatyczne uaktualnienie jest wyłączane. 
    
- **Zawieszone**: system nie jest już uprawniony do otrzymania automatycznych uaktualnień. Nie można skonfigurować tej wartości; jest on ustawiony przez system. 
    
Aby uzyskać więcej informacji zobacz temat [automatyczne uaktualnienie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Aby pobrać najnowszą wersję programu Azure AD Connect, przejdź do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

