---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736168"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz. 
  
Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:
  
- **Osiągnięto limit urządzenia** Użytkownik ma więcej zarejestrowanych urządzeń niż limit urządzenia. Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa apns (Apple Push Notification Service) musi być skonfigurowana lub odnowiona. Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby uzyskać instrukcje, jak to zrobić. 
    
- **Nieprawidłowy typ licencji użytkownika lub nazwa użytkownika nie została rozpoznana:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub Azure [portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatkowe zasoby ułatwiające rozwiązanie problemu:
  
1. Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji. 
    
2. Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązywanie problemów dla każdego z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [dokument rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Dowiedz się, jak rejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

