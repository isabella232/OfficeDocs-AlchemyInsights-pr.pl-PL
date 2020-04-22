---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759630"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.
  
Niektóre typowe problemy i kroki rozwiązywania problemów:
  
 **Błąd nieszyfrowany na urządzeniu w portalu firmy:** Nowsze wersje systemu Android, szczególnie począwszy od wersji 7.0, wymagają kodu startowego, aby upewnić się, że urządzenie jest w pełni zaszyfrowane. Typowe rozwiązania mają na celu włączenie numeru pinstart lub pełne zaszyfrowanie urządzenia. Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) aby uzyskać więcej informacji.
  
 **Urządzenia nie mogą zaewidencjonować usługi Intune lub wyświetlić jako "w złej kondycji" w konsoli administracyjnej usługi Intune:** Niektóre urządzenia Samsung 4.4 i 5.5 mogą nie zameldowyw przypadku usługi. Istnieją 3 możliwe rozwiązania tego problemu:
  
1. Ręcznie otwórz aplikację Portal firmy usługi Intune, która automatycznie zainicjuje synchronizację urządzenia.

2. Zaktualizuj urządzenie do systemu Android 6.0 lub nowszego.

3. Wyłącz program Samsung Smart Manager z zarządzania portalem firmy usługi Intune. Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) aby uzyskać więcej informacji na temat tych problemów i rozwiązań.

 **Nieprawidłowy typ licencji użytkownika** lub **błąd Nieuznany użytkownik:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: Centrum administracyjne pakietu Office lub witryny Azure portal.
  
Dodatkowe zasoby ułatwiające rozwiązanie problemu:
  
1. Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.

2. Przejrzyj [ten dokument,](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązania dla każdego z nich.

3. [Dowiedz się, jak rejestrować urządzenia z systemem Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
