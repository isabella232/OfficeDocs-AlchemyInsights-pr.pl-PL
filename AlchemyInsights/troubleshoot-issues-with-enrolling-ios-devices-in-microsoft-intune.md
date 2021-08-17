---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w aplikacji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047986"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w aplikacji Microsoft Intune

Zapoznaj się z poniższymi zasobami, aby rozwiązać problem już teraz. 
  
Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:
  
- **Osiągnięto limit urządzeń** Zarejestrowanych urządzeń jest więcej niż wynosi limit urządzeń. Przejrzyj te dokumenty, [aby usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub zmienić limit [urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta usługa nie jest obsługiwana. Bez zasad rejestracji:** Usługa wypychanych powiadomień (APNS) firmy Apple musi zostać skonfigurowana lub odnowiona. Zapoznaj [się z tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby dowiedzieć się, jak to zrobić. 
    
- **Typ licencji użytkownika Nieprawidłowy lub Nie rozpoznano nazwy użytkownika:** Użytkownikowi należy przypisać licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem witryny [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
1. Użyj [Portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji. 
    
2. Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrację i rozwiązanie dla każdego [z](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) nich: Przewodnik po rozwiązywaniu problemów i [Dokument rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Dowiedz się, jak zarejestrować urządzenia z systemem iOS w aplikacji Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

