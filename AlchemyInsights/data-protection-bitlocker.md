---
title: DataProtection — BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815625"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcji BitLocker w usłudze Intune

Zasady ochrony punktu końcowego usługi Intune mogą być używane do konfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows. Aby uzyskać więcej informacji, zobacz Ustawienia systemu [Windows 10 (lub nowszego) dotyczące](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)ochrony urządzeń za pomocą usługi Intune.

Oprócz zasad ochrony punktu końcowego istnieje również raport szyfrowania, który udostępnia bardziej szczegółowy widok stanu szyfrowania dla urządzeń. Dostęp do tego raportu można uzyskać z portalu MEM w obszarze Urządzenia **> Monitor**, a następnie w obszarze **Raport** szyfrowania konfiguracji [wybierz](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)pozycję .

Jeśli nie uda się włączyć funkcji BitLocker zgodnie z oczekiwaniami lub że profil używany do włączania funkcji BitLocker znajduje się w stanie błędu, przejrzyj raport szyfrowania, aby lepiej zrozumieć przyczynę tego zachowania.

Aby znaleźć szczegółowe informacje na temat interpretowania raportu, w tym różnych wartości stanu szyfrowania, zobacz Monitorowanie szyfrowania urządzeń [za pomocą usługi Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Należy pamiętać, że wiele nowych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie BitLocker, które jest wyzwalane bez stosowania zasad MDM. Może to mieć wpływ na stosowanie zasad, jeśli nie skonfigurowano ustawień domyślnych. Aby uzyskać więcej szczegółowych informacji, zobacz poniższe często zadawane pytania.

Aby uzyskać informacje na temat rozwiązywania problemów z funkcją bitLocker, zobacz Rozwiązywanie problemów z zasadami [funkcji BitLocker w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**CZĘSTO ZADAWANE PYTANIA**

P. Które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?<br>
O: Ustawienia w zasadach ochrony punktu końcowego usługi Intune są zaimplementowane za pomocą narzędzia [CSP funkcji BitLocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nie wszystkie wersje lub kompilacje systemu Windows obsługują program CSP funkcji BitLocker. <br><br>

P. Jak można włączyć funkcję BitLocker na urządzeniach bez konieczności wytłaniania przez użytkownika końcowego?<br>
O. Jeśli są spełnione niezbędne wymagania wstępne, można włączyć funkcję BitLocker "Silent Encryption" za pośrednictwem usługi Intune. Zapoznaj się ze szczegółami wymagań dotyczących urządzenia i przykładowymi ustawieniami zasad, aby włączyć dyskretne szyfrowanie w następującym ekwu: Dyskretne włączanie szyfrowania [funkcji BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

P. Jeśli urządzenie jest już zaszyfrowane przy użyciu funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), spowoduje to zastosowanie zasad z innymi ustawieniami automatycznie wyzwalać ponowne szyfrowanie dysku przy użyciu nowych ustawień?<br>
O: Nie. Aby zastosować nowe ustawienia szyfrowania, dysk musi najpierw zostać odszyfrowany.<br><br>
**Uwaga:** W przypadku urządzeń zarejestrowanych za pomocą rozwiązania Autopilot automatyczne szyfrowanie, które wystąpi podczas korzystania z urządzenia OOBE, nie jest wyzwalane do czasu oceny zasad usługi Intune, co pozwala na korzystanie z ustawień opartych na zasadach w miejscu wartości domyślnych systemu operacyjnego.
 
P. Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, czy zostanie odszyfrowane po usunięciu tych zasad?<br>
O. Usunięcie zasad związanych z szyfrowaniem NIE powoduje odszyfrowywania skonfigurowanych dysków.
 
P. Dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma włączonej funkcji BitLocker, mimo że jest?<br>
O: Ustawienie "Włączono funkcję BitLocker" w zasadach zgodności Usługi Intune korzysta z klienta atestacji kondycji urządzenia systemu Windows (DHA). Ten klient mierzy stan urządzenia tylko podczas rozruchu. Jeśli więc urządzenie nie zostało ponownie uruchomieniowe od momentu ukończenia szyfrowania funkcji BitLocker, usługa klienta DHA nie będzie zgłaszać funkcji BitLocker jako aktywna.
 
 