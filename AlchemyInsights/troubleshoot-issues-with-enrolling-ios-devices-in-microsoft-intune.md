---
title: Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658449"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz. 
  
Niektóre typowe komunikaty o błędach i kroki rozwiązania:
  
- **Cap urządzeń osiągnięty** Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia. Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta usługa nie jest obsługiwana. Nie zasady rejestracji:** Apple Push powiadomień usługi (APN) musi być skonfigurowany lub odnowiony. Przegląd [Ten dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) instrukcje, jak to zrobić. 
    
- **Nieprawidłowy typ licencji użytkownika ani nazwy użytkownika nie rozpoznany:** Użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS. Dokonują przeglądu tych dokumentów przypisać jedną licencję do: [Witryna Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub [portalu Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatkowe zasoby w celu rozwiązania problemu:
  
1. Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji. 
    
2. Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Informacje o sposobie rejestrowania urządzeń iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

