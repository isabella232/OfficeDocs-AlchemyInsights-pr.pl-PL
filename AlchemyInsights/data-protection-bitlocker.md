---
title: Dataprotection — funkcja BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778203"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcji BitLocker za pomocą usługi Intune

W celu skonfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows można użyć zasad usługi Intune Endpoint Protection. Aby uzyskać więcej informacji, zobacz [Ustawienia systemu Windows 10 (i nowszych wersji), aby chronić urządzenia za pomocą usługi Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Oprócz zasad ochrony punktu końcowego jest również dostępny raport dotyczący szyfrowania, który zapewnia bardziej szczegółowy widok stanu szyfrowania urządzeń. Dostęp do tego raportu można uzyskać z poziomu portalu MEM w obszarze **urządzenia > monitor**, a następnie w obszarze **Konfiguracja** wybierz [raport szyfrowania](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jeśli okaże się, że funkcja BitLocker nie zostanie włączona zgodnie z oczekiwaniami lub jeśli profil używany do włączania funkcji BitLocker jest w stanie błędu, zapoznaj się z raportem o szyfrowaniu, aby uzyskać lepsze zrozumienie przyczyny wystąpienia tego problemu.

Aby znaleźć szczegółowe informacje dotyczące interpretowania raportu zawierającego różne wartości statusu szyfrowania, zobacz [monitorowanie szyfrowania urządzenia za pomocą usługi Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji BitLocker, które zostanie wyzwolone bez zastosowania zasad MDM. Może to mieć wpływ na zastosowanie zasad, jeśli są skonfigurowane ustawienia inne niż domyślne. Aby uzyskać więcej informacji, zobacz poniższe często zadawane pytania.

Aby uzyskać informacje dotyczące rozwiązywania problemów z funkcją BitLocker, zobacz [Rozwiązywanie problemów z zasadami funkcji BitLocker w usłudze Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**CZĘSTO ZADAWANE PYTANIA**

P: Jakie wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad programu Endpoint Protection?<br>
O: ustawienia w zasadach programu Intune Endpoint Protection są implementowane przy użyciu [dostawcy CSP funkcji BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nie wszystkie wersje lub kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker. <br><br>

P: jak można włączyć funkcję BitLocker na urządzeniach bez konieczności interakcji użytkownika końcowego?<br>
O: tak długo, jak są spełnione wymagane wymagania wstępne, można włączyć funkcję BitLocker "ciche szyfrowanie" za pośrednictwem usługi Intune. Zobacz szczegółowe informacje dotyczące wymagań dotyczących urządzeń i przykładowe ustawienia zasad, aby włączyć ciche szyfrowanie w następującym dokumencie: [ciche Włączanie szyfrowania funkcji BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), zastosuje zasady z innymi ustawieniami automatycznie wyzwalają ponowne szyfrowanie dysku przy użyciu nowych ustawień?<br>
O: Nie. Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.<br><br>
**Uwaga:** W przypadku urządzeń, które są rejestrowane za pomocą funkcji autopilota, automatyczne szyfrowanie, które może wystąpić w trakcie OOBE, nie zostanie wyzwolone, dopóki nie zostanie wyznaczona zasada usługi Intune, co umożliwi użycie ustawień opartych na zasadach w miejsce ustawień domyślnych systemu operacyjnego.
 
P: Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane po usunięciu tych zasad?<br>
A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowania skonfigurowanych dysków.
 
P: dlaczego zasady zgodności usługi Intune wskazują, że na moim urządzeniu nie włączono funkcji BitLocker, mimo że jest to?<br>
A: ustawienie "włączone funkcje BitLocker" w zasadach zgodności usługi Intune korzysta z klienta usługi zaświadczeń o kondycji urządzeń systemu Windows (DHA). Ten klient mierzy tylko stan urządzenia w czasie rozruchu. Jeśli więc urządzenie nie zostało uruchomione ponownie od momentu ukończenia szyfrowania funkcją BitLocker, usługa klienta usługi DHA nie będzie raportować funkcji BitLocker jako aktywnej.
 
 