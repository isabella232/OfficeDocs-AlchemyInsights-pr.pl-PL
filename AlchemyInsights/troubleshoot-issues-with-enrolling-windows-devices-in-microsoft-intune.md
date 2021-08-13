---
title: Rozwiązywanie problemów z zarejestrowaniem Windows urządzeń w u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981051"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zarejestrowaniem Windows urządzeń w u Microsoft Intune

Zapoznaj się z poniższymi zasobami, aby rozwiązać problem już teraz.
  
Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:
  
 **Oprogramowania nie można zainstalować, można 0x80cf4017:** Certyfikat konta wygasł. Ponownie pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune. Przejrzyj tę dokumentację, aby uzyskać więcej informacji.
  
 **Kod błędu 0x801c0003:** Błąd może występować w następujących scenariuszach:
  
-  Zarejestrowanych urządzeń jest więcej niż wynosi limit urządzeń. Przejrzyj te dokumenty, [aby usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub zmienić limit [urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  Wartość "Użytkownicy mogą dołączać do urządzeń w usłudze Azure AD" jest ustawiona na wartość "brak". Ustaw ją na wszystkich lub wybranych użytkowników. Przejrzyj [tę dokumentację,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) aby uzyskać więcej informacji.

-  Urządzenie zostało już zarejestrowane przez innego użytkownika. W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie wyeminuj urządzenie przed podjęciem próby po raz kolejny.

-  Urządzenie zostanie Windows 10 Home. Tylko Windows 10 Pro, Edukacja i Enterprise mogą dołączyć do Azure Active Directory.

Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
-  Użyj [Portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.

-  Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrację i rozwiązanie dla każdego [z](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) nich: Przewodnik po rozwiązywaniu problemów i [Dokument rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Dowiedz się, jak zarejestrować Windows urządzenia w u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
