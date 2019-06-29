---
title: Rozwiązywanie problemów z zapisaniem android w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367299"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z zapisaniem android w Microsoft Intune

Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.
  
Niektóre typowe problemy i czynności rozdzielczości:
  
 **Urządzenie nie zaszyfrowany błąd w portalu firmy:** Nowsze wersje Android, szczególnie począwszy od 7.0, wymagają podania hasła uruchamiania aby upewnić się, że urządzenie jest całkowicie zaszyfrowany. Aby włączyć numer pin uruchomienia lub urządzenie w pełni szyfrowania są wspólne rozwiązania. Przegląd [Ten dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , aby uzyskać więcej informacji.
  
 **Urządzeń nie powiedzie się sprawdzanie się przy użyciu usługi Windows Intune lub wyświetlić jako "Niezdrowego" w konsoli administracyjnej usługi Intune:** Niektóre firmy Samsung 4.4 i 5.5 urządzenia nie może sprawdzić w usłudze. Istnieją 3 możliwe rozwiązania tego problemu:
  
1. Ręcznie otworzyć aplikację Portal firmy Intune, który automatycznie rozpocznie synchronizowanie urządzenia.

2. Aktualizowanie urządzenia do Android w wersji 6.0 lub nowszej.

3. Wyłączyć zarządzanie portalu Intune firmy Samsung Smart Menedżer. Przegląd [Ten dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , aby uzyskać szczegółowe informacje na temat te problemy i rozwiązania.

 **Nieprawidłowy typ licencji użytkownika** lub **użytkownika nazwa nie rozpoznany błąd:** użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS. Dokonują przeglądu tych dokumentów do przypisywania licencji za pomocą: portalu Office Admin Center lub Azure.
  
Dodatkowe zasoby w celu rozwiązania problemu:
  
1. Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.

2. Przegląd [Ten dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) lista typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego.

3. [Informacje o sposobie rejestrowania urządzeń Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
