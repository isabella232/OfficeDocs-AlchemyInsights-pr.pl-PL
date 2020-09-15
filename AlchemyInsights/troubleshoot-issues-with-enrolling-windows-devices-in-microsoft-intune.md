---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658888"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune

Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.
  
Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:
  
 **Nie można zainstalować oprogramowania, 0x80cf4017:** Twój certyfikat konta wygasł. Ponownie Pobierz pakiet oprogramowania klienckiego PC w konsoli administracyjnej usługi Intune. Aby uzyskać więcej informacji, zapoznaj się z tą dokumentacją.
  
 **Kod błędu 0x801c0003:** Błąd może wystąpić w następujących scenariuszach:
  
-  Użytkownik ma więcej urządzeń zarejestrowanych poza limitem urządzeń. Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Użytkownicy mogą dołączać do urządzeń w usłudze Azure AD" ma ustawioną wartość "Brak". Ustaw go na wszystkich lub wybierz pozycję Użytkownicy. Aby uzyskać więcej informacji, zapoznaj się z [tą dokumentacją](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Urządzenie zostało już zarejestrowane przez innego użytkownika. W takim przypadku Usuń urządzenie z konsoli Azure Intune lub ręcznie odrejestrowania urządzenia przed ponowną próbą.

-  Urządzenie to Windows 10 Home. Do usługi Azure Active Directory można dołączyć tylko wersje Windows 10 Pro, Education i Enterprise.

Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
-  Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.

-  Przejrzyj te dokumenty, aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie [problemów z](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)każdym z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) .

[Dowiedz się, jak zarejestrować urządzenia z systemem Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
