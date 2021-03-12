---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708900"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.
  
Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:
  
 **Nie można zainstalować oprogramowania, 0x80cf4017:** Certyfikat konta wygasł. Ponownie pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune. Aby uzyskać więcej informacji, zapoznaj się z tą dokumentacją.
  
 **Kod błędu 0x801c0003:** Błąd może występować w następujących scenariuszach:
  
-  Użytkownik ma zarejestrowanych więcej urządzeń niż wynosi limit urządzeń. Przejrzyj te dokumenty, [aby usunąć urządzenie lub](https://docs.microsoft.com/intune/devices-wipe) zmienić limit [urządzeń.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Ustawienie "Użytkownicy mogą dołączać urządzenia do usługi Azure AD" ma wartość "brak". Ustaw ją na wszystkich lub wybierz użytkowników. Aby [uzyskać więcej informacji,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) zapoznaj się z tą dokumentacją.

-  Urządzenie zostało już zarejestrowane przez innego użytkownika. W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie usuń je przed podjęciem próby.

-  Urządzenie to Windows 10 Home. Do usługi Azure Active Directory mogą dołączyć tylko jednostki SKU systemu Windows 10 Pro, Education i Enterprise.

Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
-  Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.

-  Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrowanie i rozwiązywanie poszczególnych [problemów:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) przewodnik po rozwiązywaniu problemów i dokument [rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Dowiedz się, jak zarejestrować urządzenia z systemem Windows w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
