---
title: Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555303"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta

Profile certyfikatów klienta usługi Intune NDES/SCEP i PKCS/PFX są powszechnie używane w połączeniu z innymi typami profili, takimi jak Wifi, VPN i poczta e-mail, aby umożliwić użytkownikom uwierzytelnienie się w zasobach firmowych. Gdy te typy profili są połączone z profilem certyfikatu klienta są zależne od pomyślnego wdrożenia tego profilu.

Początkowa konfiguracja infrastruktury i skojarzona konfiguracja profilu certyfikatu klienta często wymagają rozwiązywania problemów. Aby uzyskać przewodnik krok po kroku dotyczący pomyślnej konfiguracji łącznika NDES i wskazówek dotyczących rozwiązywania problemów w celu wyizolowania problemów z wdrażaniem certyfikatów, zobacz: 

- [Konfigurowanie infrastruktury do obsługi narzędzia SCEP w usłudze Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Użyj skryptów programu PowerShell, do których odwołuje się skrypty programu PowerShell, aby zweryfikować konfigurację. Aby uzyskać więcej informacji, zobacz [Skrypty weryfikacji łącznika łącznika usługi Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Inne typowe problemy**

**Podczas próby zainstalowania łącznika certyfikatu usługi Intune na serwerze łącznika NDES otrzymuję komunikat "Nie można zweryfikować hasła w żądaniu certyfikatu. Być może był już używany. Uzyskaj nowe hasło do przesłania z tym żądaniem."**  

Ten komunikat oznacza, że należy uruchomić instalację łącznika certyfikatu jako administrator.

W niektórych środowiskach serwery uruchamiane jako certyfikat usługi Intune muszą używać serwera proxy do łączenia się z usługą Intune, dlatego łącznik certyfikatów musi używać serwera proxy. W pewnych okolicznościach łącznik NDES ignoruje skonfigurowane ustawienia serwera proxy i może być konieczne skonfigurowanie ustawień serwera proxy podczas uruchamiania w kontekście zabezpieczeń systemu localsystem. 
 
Rozwiązaniem jest uruchomienie programu Internet Explorer jako system i skonfigurowanie serwera proxy w programie IE. Po ponownym uruchomieniu usługi łącznika usługi Intune łącznik ndes łącznik łączy się z usługą Intune.

**Urządzenia użytkownika nie otrzymują już certyfikatów SCEP od NDES.**

Możliwe, że certyfikat uwierzytelniania klienta wystawiony serwerowi NDES i określony podczas instalacji łącznika NDES wygasł lub jej brakuje. Aby rozwiązać: 
 
1. Odinstaluj łącznik NDES.  
2. Te szczegóły można użyć, aby zażądać nowego certyfikatu uwierzytelniania klienta lub certyfikatu uwierzytelniania serwera: 
 
    - Nazwa podmiotu: CN =external fqdn  
    - Alternatywna nazwa podmiotu (obie są wymagane): DNS=external fqdn, DNS=internal fqdn 
 
3. Zainstaluj ponownie łącznik NDES z nowym certyfikatem.