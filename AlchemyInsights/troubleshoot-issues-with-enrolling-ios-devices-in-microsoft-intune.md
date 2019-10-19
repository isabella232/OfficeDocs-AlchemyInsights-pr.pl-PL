---
title: Rozwiązywanie problemów z rejestrowanie urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507013"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowanie urządzeń z systemem iOS w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz. 
  
Niektóre typowe komunikaty o błędach i kroki rozwiązania:
  
- **Osiągnięto limit urządzenia** Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia. Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa powiadomień wypychanych firmy Apple (APNS) musi być skonfigurowana lub odnawiana. Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , aby uzyskać instrukcje, jak to zrobić. 
    
- **Typ licencji użytkownika nieprawidłowy lub nie rozpoznano nazwy użytkownika:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatkowe zasoby ułatwiające rozwiązanie problemu:
  
1. Używaj [portalu rozwiązywania problemów z usługą Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) do diagnozowania i rozwiązywania typowych błędów rejestracji. Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji. 
    
2. Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrowanie i rozwiązania dla każdego: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [dokument dotyczący rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Dowiedz się, jak rejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

