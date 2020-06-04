---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665842"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.
  
Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:
  
 **Nie można zainstalować oprogramowania, 0x80cf4017:** Certyfikat konta wygasł. Pobierz ponownie pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune. Zapoznaj się z tą dokumentacją, aby uzyskać więcej informacji.
  
 **Kod błędu 0x801c0003:** Błąd może wystąpić w następujących scenariuszach:
  
-  Użytkownik ma więcej zarejestrowanych urządzeń niż limit urządzenia. Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Użytkownicy mogą dołączyć do urządzeń do usługi Azure AD" jest ustawiona na "brak". Ustaw go na wszystkich lub wybierz użytkowników. Zapoznaj się z [tą dokumentacją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) aby uzyskać więcej informacji.

-  Urządzenie jest już zarejestrowane przez innego użytkownika. W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie wyrejestruj urządzenie przed ponowną próbą.

-  Urządzenie jest Windows 10 Home. Tylko jednostki SKU systemu Windows 10 Pro, Education i Enterprise mogą dołączyć do usługi Azure Active Directory.

Dodatkowe zasoby ułatwiające rozwiązanie problemu:
  
-  Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.

-  Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązywanie problemów dla każdego z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [dokument rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Dowiedz się, jak rejestrować urządzenia z systemem Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
