---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708972"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem. 
  
Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:
  
- **Osiągnięto limit urządzeń** Użytkownik ma zarejestrowanych więcej urządzeń niż wynosi limit urządzeń. Przejrzyj te dokumenty, [aby usunąć urządzenie lub](https://docs.microsoft.com/intune/devices-wipe) zmienić limit [urządzeń.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ta usługa nie jest obsługiwana. Bez zasad rejestracji:** usługa powiadomień push firmy Apple (APNS) wymaga skonfigurowania lub odnowienia. Zapoznaj [się z tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby uzyskać instrukcje dotyczące tego, jak to zrobić. 
    
- **Nieprawidłowy typ licencji użytkownika lub nie rozpoznano nazwy użytkownika:** Użytkownikowi musi być przypisana licencja usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Centrum administracyjnego pakietu Office](https://docs.microsoft.com/intune/licenses-assign) lub Portalu [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
1. Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji. 
    
2. Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrowanie i rozwiązywanie poszczególnych [problemów:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) przewodnik po rozwiązywaniu problemów i dokument [rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Dowiedz się, jak zarejestrować urządzenia z systemem iOS w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

