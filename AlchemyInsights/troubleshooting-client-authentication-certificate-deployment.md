---
title: Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020814"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta

Profile klientów NDES/SCEPT i PKCS/PFX Intune są często używane w połączeniu z innymi typami profilów, takimi jak sieć Vpn i poczta e-mail, aby umożliwić użytkownikom uwierzytelnienie się w zasobach firmowych. To, czy te typy profilów są połączone z profilem certyfikatu klienta, zależy od pomyślnego wdrożenia tego profilu.

Początkowa konfiguracja infrastruktury i skojarzona konfiguracja profilu certyfikatu klienta często wymagają rozwiązania problemów. Aby uzyskać przewodnik krok po kroku dotyczący pomyślnego konfigurowania łącznika NDES i rozwiązywania problemów w celu wyizolowania problemów przy użyciu wdrożenia certyfikatu, zobacz: 

- [Konfigurowanie infrastruktury pod celu obsługi danych SCEPT za pomocą usługi Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Omówienie rozwiązywania problemów z profilami certyfikatów SCEPT za pomocą Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Użyj skryptów programu PowerShell, do których się odwołujesz, aby zweryfikować konfigurację. Aby uzyskać więcej informacji, zobacz Skrypty weryfikacyjne [łącznika certyfikatu usługi Intune.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Inne typowe problemy**

**Podczas próby zainstalowania łącznika certyfikatu usługi Intune na serwerze łącznika NDES jest wyświetlany komunikat "Nie można zweryfikować hasła w żądaniu certyfikatu. Być może już go używano. Uzyskaj nowe hasło, aby przesłać to żądanie".**  

Ten komunikat oznacza, że musisz uruchomić instalację łącznika certyfikatu jako administrator.

W niektórych środowiskach serwery, na których jest uruchamiany certyfikat usługi Intune, muszą łączyć się z usługą Intune za pomocą serwera proxy, a więc łącznik certyfikatu musi używać serwera proxy. W pewnych okolicznościach łącznik NDES ignoruje skonfigurowane ustawienia serwera proxy i może być konieczne skonfigurowanie ustawień serwera proxy podczas uruchamiania w kontekście zabezpieczeń LocalSystem. 
 
Rozwiązaniem jest uruchomienie programu Internet Explorer jako systemu i skonfigurowanie serwera proxy w programie Internet Explorer. Po ponownym uruchomieniu usługi Intune Connector łącznik NDES łączy się z usługą Intune.

**Urządzenia użytkowników nie otrzymują już certyfikatów SCEPT od NDES.**

Istnieje możliwość, że certyfikat uwierzytelniania klienta wystawiony dla serwera NDES i określony podczas instalacji łącznika NDES wygasł lub nie istnieje. Aby rozwiązać problem: 
 
1. Odinstaluj łącznik NDES.  
2. Skorzystaj z tych informacji, aby zażądać nowego uwierzytelniania klienta lub certyfikatu uwierzytelniania serwera: 
 
    - Nazwa tematu: CN=zewnętrzna nazwa fqdn  
    - Nazwa alternatywna tematu (wymagane są obie nazwy): DNS=zewnętrzna nazwa fqdn, DNS=wewnętrzna nazwa fqdn 
 
3. Ponownie zainstaluj łącznik NDES za pomocą nowego certyfikatu.