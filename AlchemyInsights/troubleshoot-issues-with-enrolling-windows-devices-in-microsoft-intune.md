---
title: Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390653"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz. 
  
Niektóre typowe komunikaty o błędach i kroki rozwiązania:
  
 **Nie można zainstalować oprogramowania, 0x80cf4017:** Twój certyfikat konta wygasło. Ponownie Pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune. Przejrzyj tę dokumentację, aby uzyskać więcej informacji. 
  
 **Kod błędu 0x801c0003:** Ten błąd może wystąpić w następujących scenariuszach: 
  
1. Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia. Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Użytkownicy mogą przyłączyć urządzenia do Azure AD" jest ustawiony na "Brak". Ustaw go na wszystkie lub wybierz użytkowników. Przegląd [tej dokumentacji](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , aby uzyskać więcej informacji. 
    
3. Urządzenie jest już zarejestrowane przez innego użytkownika. Jeśli tak się stanie, usuń urządzenie z konsoli Azure Intune lub ręcznie anulować rejestrację urządzenia przed ponowną próbą.
    
4. Urządzenie jest Windows 10 strona główna. Tylko Windows 10 Pro, edukacji i wersji Enterprise można przyłączyć Azure usługi Active Directory.
    
Dodatkowe zasoby w celu rozwiązania problemu:
  
1. Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji. 
    
2. Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Informacje o sposobie rejestrowania urządzeń systemu Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

