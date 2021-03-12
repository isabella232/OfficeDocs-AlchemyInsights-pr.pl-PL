---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709008"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.
  
Niektóre typowe problemy i procedury rozwiązywania problemów:
  
 **Błąd urządzenia, który nie jest zaszyfrowany w portalu firmy:** Nowsze wersje systemu Android, zwłaszcza począwszy od wersji 7.0, wymagają kodu dostępu podczas uruchamiania, aby upewnić się, że urządzenie jest w pełni zaszyfrowane. Typowe rozwiązania to włączenie numeru PIN startowego lub pełne zaszyfrowanie urządzenia. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) aby uzyskać więcej informacji.
  
 Urządzenia nie mogą się sprawdzić za pomocą usługi Intune lub są wyświetlane jako **"Zła kondycja" w konsoli administracyjnej Intune:** Niektóre urządzenia z systemem Samsung 4.4 i 5.5 mogą nie sprawdzić się w usłudze. Istnieją 3 możliwe rozwiązania tego problemu:
  
1. Ręcznie otwórz aplikację portalu firmy Intune, która automatycznie zainicjuje synchronizację urządzeń.

2. Zaktualizuj urządzenie do wersji Android 6.0 lub wyższej.

3. Wyłącz funkcję Samsung Smart Manager z zarządzania portalem firmy Intune. Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) aby uzyskać szczegółowe informacje na temat tych problemów i ich rozwiązywania.

 **Błąd "Nieprawidłowy typ** licencji użytkownika" lub "Nazwa użytkownika nie rozpoznano": użytkownikowi należy przypisać licencję usługi Intune lub EMS.  Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: Centrum administracyjnego pakietu Office lub Portalu Azure.
  
Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
1. Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.

2. Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązanie każdego z nich.

3. [Dowiedz się, jak zarejestrować urządzenia z systemem Android w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
