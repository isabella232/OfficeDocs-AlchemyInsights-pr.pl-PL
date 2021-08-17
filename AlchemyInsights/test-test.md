---
title: Brak warunków w SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106436"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcji BitLocker w usłudze Intune

Zasady Endpoint Protection Intune mogą być używane do konfigurowania ustawień szyfrowania BoitLocker dla urządzeń Windows w sposób opisany w : Ustawieniach systemu Windows10 (lub nowszych) w celu ochrony urządzeń za pomocą usługi Intune

Należy pamiętać, że wiele nowych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie bitLocker, które jest wyzwalane bez stosowania zasad MDM. Może to mieć wpływ na stosowanie zasad, jeśli nie skonfigurowano ustawień domyślnych. Aby uzyskać więcej szczegółowych informacji, zobacz Często zadawane pytania.


Często zadawane pytania: Które wersje aplikacji Windows obsługują szyfrowanie urządzeń przy użyciu Endpoint Protection zabezpieczeń?
O: Ustawienia w usłudze Intune Endpoint Protection są zaimplementowane przy użyciu narzędzia CSP funkcji BitLocker.  Nie wszystkie wersje ani kompilacje aplikacji Windows obsługują usługę CSP funkcji BitLocker. Obecnie są Windows: Enterprise; Aplikacje Education, Mobile, Mobile Enterprise i Professional (od kompilacji 1809 dalej) są obsługiwane.




P. Jeśli urządzenie jest już zaszyfrowane przy użyciu funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), spowoduje to zastosowanie zasad z innymi ustawieniami automatycznie wyzwalać ponowne szyfrowanie dysku przy użyciu nowych ustawień?

Odp. Nie. Aby zastosować nowe ustawienia szyfrowania, dysk musi najpierw zostać odszyfrowany.

Uwaga W przypadku urządzeń zarejestrowanych za pomocą rozwiązania Autopilot automatyczne szyfrowanie, które wystąpi podczas korzystania z urządzenia OOBE, nie zostanie wyzwolone do czasu oceny zasad usługi Intune, co pozwala na korzystanie z ustawień opartych na zasadach w miejscu wartości domyślnych systemu operacyjnego




P Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane, gdy te zasady zostaną usunięte?

O. Usunięcie zasad związanych z szyfrowaniem NIE powoduje odszyfrowywania skonfigurowanych dysków.




P. Dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma włączonej funkcji BitLocker, ale tak jest?

O: Ustawienie "Włączono funkcję BitLocker" w zasadach zgodności usługi Intune korzysta z klienta Windows Kondycja urządzeń (DHA). Ten klient mierzy stan urządzenia tylko podczas rozruchu. Jeśli więc urządzenie nie zostało ponownie rozruchu po zakończeniu szyfrowania funkcją bitLocker, usługa klienta DHA nie będzie zgłaszać funkcji bitLocker jako aktywna.