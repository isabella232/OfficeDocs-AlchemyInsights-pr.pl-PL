---
title: Brakuje terminów w magazynie terminów usługi SharePoint Online
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750461"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Włączanie szyfrowania funkcji BitLocker za pomocą usługi Intune

Zasady usługi Intune Endpoint Protection mogą być używane do konfigurowania ustawień szyfrowania Boitlocker dla urządzeń z systemem Windows, zgodnie z opisem w następujących systemach: Windows10 (i nowszych) w celu ochrony urządzeń przy użyciu usługi Intune.

Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji BitLocker, które zostanie wyzwolone bez zastosowania zasad MDM. Może to mieć wpływ na zastosowanie zasad, jeśli nie skonfigurowano ustawień niedomyślnych. Zobacz często zadawane pytania, aby uzyskać więcej szczegółowych informacji.


Często zadawane pytania   p: Jakie wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad programu Endpoint Protection?
 O: ustawienia w zasadach programu Intune Endpoint Protection są implementowane przy użyciu dostawcy CSP funkcji BitLocker.Nie wszystkie wersje i kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker. 
      W tym momencie wersja systemu Windows: Enterprise; Obsługiwane są wykształcenie, telefony komórkowe, telefony komórkowe i profesjonalne (od kompilacji 1809).




P: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), będą stosowane zasady z różnymi ustawieniami automatycznie wyzwalać ponowne szyfrowanie dysku przy użyciu nowych ustawień?

O: Nie. Aby zastosować nowe ustawienia szyfru, należy najpierw odszyfrować dysk.

Uwaga dotycząca urządzeń zarejestrowanych za pomocą autopilota automatyczne szyfrowanie, które może wystąpić w trakcie OOBE, nie zostanie wyzwolone, dopóki nie zostanie wykryta zasada usługi Intune, która zezwala na użycie ustawień opartych na zasadach w miejscu domyślnym systemu operacyjnego




P Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane po usunięciu tych zasad?

A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowania dysków, które zostały skonfigurowane.




P: dlaczego zasady zgodności usługi Intune wskazują, że na moim urządzeniu nie włączono funkcji "BitLocker Enabled", ale jest to?

A: ustawienie "włączone funkcje BitLocker" w zasadach zgodności usługi Intune korzysta z klienta usługi zaświadczeń o kondycji urządzeń systemu Windows (DHA). Ten klient mierzy tylko stan urządzenia w czasie rozruchu. Jeśli więc urządzenie nie zostało uruchomione ponownie od momentu ukończenia szyfrowania funkcją BitLocker, usługa klienta DHA nie będzie raportować funkcji BitLocker jako aktywnej.