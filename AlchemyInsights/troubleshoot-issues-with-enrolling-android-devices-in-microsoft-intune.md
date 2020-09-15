---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689964"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune

Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.
  
Oto niektóre typowe problemy i rozwiązywanie problemów:
  
 **Błąd urządzenia nie zaszyfrowano w portalu firmy:** Nowsze wersje systemu Android, szczególnie w przypadku rozpoczynania pracy z wersją v 7.0, wymagają kodu dostępu, aby upewnić się, że urządzenie jest w pełni szyfrowane. Typowe rozwiązania to włączenie numeru PIN uruchamiania lub pełnego zaszyfrowania urządzenia. Przejrzyj [ten dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , aby uzyskać więcej informacji.
  
 **Urządzenia nie zapoznają się z usługą Intune ani wyświetlać jako "niezdrowe" w konsoli administracyjnej usługi Intune:** Niektóre urządzenia Samsung 4,4 i 5,5 mogą nie zaewidencjonować usługi. Istnieją 3 możliwe rozwiązania tego problemu:
  
1. Ręcznie otwórz aplikację Portal firmy usługi Intune, co spowoduje automatyczne zainicjowanie synchronizacji urządzenia.

2. Zaktualizuj urządzenie do wersji Android 6,0 lub nowszej.

3. Wyłączenie zarządzania portalem firmowym usługi Intune przy użyciu usługi Samsung Smart Manager. Przejrzyj [ten dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , aby uzyskać więcej informacji o tych problemach i rozwiązaniach.

 **Typ licencji użytkownika jest nieprawidłowy** lub **Nazwa użytkownika nie została rozpoznana. błąd:** użytkownik musi mieć przypisaną licencję usługi Intune lub EMS. Przejrzyj te dokumenty, aby przypisać licencję: Centrum administracyjne pakietu Office lub Azure Portal.
  
Dodatkowe zasoby pomocne w rozwiązaniu problemu:
  
1. Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.

2. Przejrzyj [ten dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie problemów.

3. [Dowiedz się, jak zarejestrować urządzenia z systemem Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
