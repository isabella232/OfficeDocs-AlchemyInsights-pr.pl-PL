---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669258"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune

Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz. 
  
Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:
  
- **Osiągnięto koniec urządzenia** Użytkownik ma więcej urządzeń zarejestrowanych poza limitem urządzeń. Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa Apple Push Notification Service (APN) musi być skonfigurowana lub odnawiana. Przejrzyj [ten dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , aby uzyskać instrukcje dotyczące wykonywania tej czynności. 
    
- **Typ licencji użytkownika jest nieprawidłowy lub nie rozpoznano nazwy użytkownika:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję: [Centrum administracyjne pakietu Office](https://docs.microsoft.com/intune/licenses-assign) lub [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
1. Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji. 
    
2. Przejrzyj te dokumenty, aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie [problemów z](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)każdym z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) .
    
3. [Dowiedz się, jak zarejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

