---
title: Testowanie konfiguracji usługi IRM pod celu przetestowania nowych funkcji usługi OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812442"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testowanie konfiguracji usługi IRM pod celu przetestowania nowych funkcji usługi OME

Aby sprawdzić, czy dzierżawa usługi Microsoft 365 jest skonfigurowana do korzystania z nowych funkcji OME, uruchom następujące polecenia cmdlet podczas połączenia z [programem Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Sprawdź konfigurację usługi IRM dzierżawy, uruchamiając program `Get-IRMConfiguration` . Upewnij się, że dla tych wartości ustawiono wartość **Prawda:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Uruchom za pomocą swojej domeny, adresu nadawcy i adresata `Test-IRMConfiguration` . Jeśli test nie przejdzie, zbadaj konfigurację usługi IRM.

Aby uzyskać więcej informacji na temat weryfikowania konfiguracji usługi IRM, zobacz Weryfikowanie nowej konfiguracji usługi OME w [programie Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)