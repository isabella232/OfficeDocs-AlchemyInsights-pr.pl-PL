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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658996"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rozwiązywanie problemów z wdrażaniem certyfikatu uwierzytelniania klienta

Profile certyfikatów klienta usługi Intune NDES/SCEP i PKCS/PFX są często używane w połączeniu z innymi typami profilów, takimi jak WiFi, VPN i poczta e-mail, aby umożliwić użytkownikom uwierzytelnianie w zasobach firmowych. Jeśli te typy profilów są połączone z profilem certyfikatu klienta, są zależne od poprawnego wdrożenia tego profilu.

Początkowa konfiguracja infrastruktury i skojarzona konfiguracja profilu certyfikatu klienta wymagają często rozwiązywania problemów. Aby zapoznać się z przewodnikiem krok po kroku dotyczącym poprawnego konfigurowania łącznika usługi NDES i wskazówek dotyczących rozwiązywania problemów z wdrażaniem certyfikatów, zobacz: 

- [Konfigurowanie infrastruktury do obsługi protokołu SCEP za pomocą usługi Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Używanie skryptów programu PowerShell, do których można sprawdzić konfigurację. Aby uzyskać więcej informacji, zobacz [skrypty weryfikacji łącznika certyfikatów usługi Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Inne typowe problemy**

**Gdy próbuję zainstalować łącznik certyfikatów usługi Intune na serwerze usługi NDES Connector, jest wyświetlany komunikat "nie można zweryfikować hasła w żądaniu certyfikatu. Być może został on już wykorzystany. Uzyskaj nowe hasło do przesłania za pomocą tego żądania.**  

Ta wiadomość oznacza, że musisz uruchomić instalację łącznika certyfikatu jako administrator.

W niektórych środowiskach serwery, na których jest uruchomiony certyfikat usługi Intune, muszą używać serwera proxy do nawiązywania połączenia z usługą Intune, więc łącznik certyfikatów musi używać serwera proxy. W pewnych okolicznościach łącznik usługi NDES ignoruje skonfigurowane ustawienia serwera proxy i może być konieczne skonfigurowanie ustawień serwera proxy podczas uruchamiania w kontekście zabezpieczeń LocalSystem. 
 
Rozwiązanie polega na uruchomieniu programu Internet Explorer w systemie i skonfigurowaniu serwera proxy w programie IE. Po ponownym uruchomieniu usługi łącznika usługi Intune łącznik usługi NDES łączy się z usługą Intune.

**Urządzenia użytkowników nie odbierają już certyfikatów SCEP z usługi NDES.**

Możliwe, że certyfikat uwierzytelniania klienta wystawiony dla serwera NDES i określony podczas instalacji łącznika usługi NDES stracił ważność lub go brakuje. Aby rozpoznać: 
 
1. Odinstaluj łącznik usługi NDES.  
2. Te szczegóły umożliwiają zażądanie nowego uwierzytelniania klienta lub certyfikatu uwierzytelniania serwera: 
 
    - Nazwa podmiotu: CN = zewnętrzna nazwa FQDN  
    - Alternatywna nazwa podmiotu (wymagane): DNS = zewnętrzna nazwa FQDN, DNS = wewnętrzna nazwa FQDN 
 
3. Ponownie zainstaluj łącznik usługi NDES z nowym certyfikatem.