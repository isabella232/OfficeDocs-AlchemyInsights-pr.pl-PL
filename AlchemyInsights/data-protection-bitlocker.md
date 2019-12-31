---
title: DataProtection — funkcja BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908719"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcją BitLocker w usłudze Intune

 Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows. Aby uzyskać więcej informacji, zobacz [Ustawienia systemu Windows 10 (i nowsze), aby chronić urządzenia przy użyciu usługi Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcją BitLocker, który jest wyzwalany bez stosowania zasad MDM. Może to wpłynąć na stosowanie zasad, jeśli skonfigurowano inne niż domyślne ustawienia. Zobacz następujące FAQ, aby uzyskać więcej szczegółów.
 
Aby uzyskać informacje dotyczące rozwiązywania problemów z funkcją BitLocker, zobacz Rozwiązywanie problemów z [zasadami funkcji BitLocker w usłudze Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Często zadawane pytania**

 P: które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?<br>
 A: ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu [dostawcy CSP funkcji BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nie wszystkie edycje lub kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker. <br><br>
      W tej chwili obsługiwane są następujące wersje systemu Windows: Enterprise, edukacja, komórka, Mobile Enterprise i Professional (kompilacja 1809 i nowsze).
 
Q: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfru (XTS-AES-128), będzie stosowanie zasad z różnych ustawień automatycznie wyzwolić ponowne szyfrowanie dysku z nowymi ustawieniami?<br>
O: nie. Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.<br><br>
**Uwaga:** W przypadku urządzeń zarejestrowanych w programie autopilot automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostanie oszacowana zasada usługi Intune, co umożliwi ustawienia oparte na zasadach, które będą używane zamiast ustawień domyślnych systemu operacyjnego.
 
P: Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie ono odszyfrowane po usunięciu tej zasady?<br>
A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowywania dysków, które zostały skonfigurowane.
 
Q: dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma włączoną funkcją BitLocker, mimo że jest?<br>
A: ustawienie "włączona funkcja BitLocker" w zasadach zgodności usługi Intune korzysta z klienta Windows Device atestacja zdrowia (DHA). Ten klient mierzy tylko stan urządzenia w czasie rozruchu. Jeśli więc urządzenie nie zostało ponownie uruchomiony od czasu ukończenia szyfrowania funkcją BitLocker, usługa klienta DHA nie będzie raportować funkcji BitLocker jako aktywnej.
 
 