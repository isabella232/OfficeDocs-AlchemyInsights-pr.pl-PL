---
title: Nie skonfigurowano certyfikatu Apple MDM Push Certificate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440015"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Nie skonfigurowano certyfikatu Apple MDM Push Certificate

Certyfikat push apple MDM (znany również jako certyfikat apns (Apple Push Notification Service) nie został skonfigurowany dla subskrypcji. Bez skonfigurowanego certyfikatu push urządzenia mdm systemu Apple MDM nie można rejestrować urządzeń z systemem iOS i Mac OS i zarządzać nimi. Po dodaniu certyfikatu do usługi Intune użytkownicy mogą zainstalować aplikację Portal firmy, aby zarejestrować swoje urządzenia z systemem iOS.

1. Wybierz **"Zgadzam się".** , aby udzielić firmie Microsoft uprawnień do wysyłania danych do firmy Apple.

2. Wybierz **pozycję Pobierz csr** żądanie podpisywania certyfikatu usługi Intune wymagane do utworzenia certyfikatu wypychania urządzenia Apple MDM. Plik jest używany do żądania certyfikatu relacji zaufania z portalu Apple Push Certificates Portal.

3. Wybierz **pozycję Utwórz certyfikat wypychania mdm,** aby przejść do portalu Apple Push Certificates Portal. Zaloguj się za pomocą firmowego konta Apple ID, a następnie wybierz pozycję **Utwórz certyfikat**. Wybierz **pozycję Wybierz plik**, przejdź do pliku żądania podpisywania certyfikatu, a następnie wybierz pozycję **Przekaż**. Na stronie Potwierdzenie wybierz pozycję **Pobierz,** aby pobrać plik certyfikatu (pem), a następnie zapisz plik lokalnie.
 
**Uwaga:** Certyfikat jest skojarzony z identyfikatorem Apple ID użytym do jego utworzenia. Najlepszym rozwiązaniem jest używanie firmowego konta Apple ID do zadań zarządzania i upewnienie się, że skrzynka pocztowa jest monitorowana przez więcej niż jedną osobę lub przy użyciu listy dystrybucyjnej. Nigdy nie używaj osobistego konta Apple ID. Użyj tego samego konta Apple ID, aby odnawiać certyfikat Apple Push co 12 miesięcy.
 
4. Wprowadź identyfikator Apple ID użyty do utworzenia certyfikatu wypychania urządzenia Apple MDM. Zapisz ten identyfikator jako przypomnienie, gdy trzeba odnowić certyfikat.

5. Przejdź do pliku certyfikatu (pem), wybierz pozycję **Otwórz**, a następnie wybierz pozycję **Przekaż**. Dzięki certyfikatowi wypychania usługa Intune może rejestrować urządzenia firmy Apple i zarządzać nimi.