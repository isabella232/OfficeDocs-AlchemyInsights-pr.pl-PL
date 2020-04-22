---
title: Terminy, na które brakuje w sklepie terminowym usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766863"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcji Bitlocker za pomocą usługi Intune

Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania boitlocker dla urządzeń z systemem Windows, jak opisano w : Ustawienia systemu Windows10 (i nowsze) w celu ochrony urządzeń korzystających z usługi Intune

Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji bitlocker, które jest wyzwalane bez stosowania zasad MDM. Może to mieć wpływ na stosowanie zasad, jeśli skonfigurowano ustawienia domyślne. Zobacz często zadawane pytania, aby uzyskać więcej informacji.


Często  zadawane pytania P: Które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?
 Odp.: Ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu usługi CSP funkcji Bitlocker.Nie wszystkie wersje ani kompilacje systemu Windows obsługują CSP funkcji Bitlocker. 
      W tej chwili Windows Editions: Enterprise; Edukacja, Mobile, Mobile Enterprise i Professional (od kompilacji 1809 i 1809) są obsługiwane.




Pyt.: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji Bitlocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), zastosuje zasadę z różnymi ustawieniami automatycznie wyzwala ponowne szyfrowanie dysku z nowymi ustawieniami?

Odp.: Nie. Aby zastosować nowe ustawienia szyfrowania, dysk musi najpierw zostać odszyfrowany.

Uwaga W przypadku urządzeń zarejestrowanych za pomocą autopilota automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostaną ocenione zasady usługi Intune, które umożliwiają użycie ustawień opartych na zasadach zamiast ustawień systemu operacyjnego




P Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie ono odszyfrowane po usunięciu tej zasady?

Odp.: Usunięcie zasad związanych z szyfrowaniem NIE powoduje odszyfrowania dysków, które zostały skonfigurowane.




Pyt.: Dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma funkcji "Bitlocker Enabled", ale tak jest?

Odp.: Ustawienie "Funkcja blokowania bitów włączone" w zasadach zgodności usługi Intune wykorzystuje klienta zaświadczania kondycji urządzenia systemu Windows (DHA). Ten klient mierzy tylko stan urządzenia w czasie rozruchu. Jeśli więc urządzenie nie zostało ponownie uruchomione od czasu zakończenia szyfrowania funkcji bitlocker, usługa klienta DHA nie będzie zgłaszać funkcji bitlocker jako aktywnej.