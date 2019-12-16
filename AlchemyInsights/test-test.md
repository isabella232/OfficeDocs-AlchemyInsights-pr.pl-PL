---
title: Terminy brakujące w usłudze SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053523"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcją BitLocker w usłudze Intune

Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania Boitlocker dla urządzeń z systemem Windows zgodnie z opisem w: ustawienia Windows10 (i nowsze) w celu ochrony urządzeń przy użyciu usługi Intune

Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcją BitLocker, który jest wyzwalany bez stosowania zasad MDM. Może to wpłynąć na stosowanie zasad, jeśli nie skonfigurowano ustawień domyślnych. Więcej szczegółów znajdziesz w FAQ.


Często  zadawane pytania Q: które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?
 A: ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu programu CSP funkcji BitLocker.Nie wszystkie edycje ani kompilacje systemu Windows nie obsługują programu CSP funkcji BitLocker. 
      W tej chwili wersje systemu Windows: Enterprise; Edukacja, komórka, Mobile Enterprise i Professional (od Build 1809 i nowsze) są obsługiwane.




Q: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfru (XTS-AES-128) będzie stosowanie zasad z różnych ustawień automatycznie wyzwolić ponowne szyfrowanie dysku z nowymi ustawieniami?

O: nie. Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.

Uwaga w przypadku urządzeń zarejestrowanych w programie autopilot automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostanie oszacowana zasada usługi Intune, która zezwala na korzystanie z ustawień opartych na zasadach zamiast wartości domyślnych systemu operacyjnego




Q Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune zostanie on odszyfrowany po usunięciu tej zasady?

A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowywania dysków, które zostały skonfigurowane.




P: dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma "włączoną funkcją BitLocker", ale jest?

A: ustawienie "włączona funkcja BitLocker" w zasadach zgodności usługi Intune korzysta z klienta Windows Device Health atestacja (DHA). Ten klient mierzy tylko stan urządzenia w czasie rozruchu. Jeśli więc urządzenie nie zostało ponownie uruchomiony, ponieważ szyfrowanie funkcją BitLocker zostało zakończone, usługa klienta DHA nie zgłosi funkcji BitLocker jako aktywnej.