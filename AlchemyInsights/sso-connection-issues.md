---
title: Problemy z połączeniem logowania jednokrotnego
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935155"
---
# <a name="sso-connection-issues"></a>Problemy z połączeniem logowania jednokrotnego

1. Postępuj zgodnie [z oknie Szybki start: konfigurowanie właściwości przewodnika aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) w celu skonfigurowania aplikacji.
2. W zależności od wybranej [aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) i opcji logowania pojedynczego postępuj zgodnie z poniższymi wskazówkami:
    - Aby skonfigurować aplikację **lokalną dla** logowania pojedynczego opartego na forach **SAML,** zobacz logowanie pojedyncze SAML dla aplikacji lokalnych z serwerem [proxy aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Aby skonfigurować aplikację **w chmurze** do logowania pojedynczego opartego na **hasłach,** zobacz Konfigurowanie logowania pojedynczego [hasła.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Aby skonfigurować aplikację **lokalną dla** logowania pojedynczego za pośrednictwem serwera **proxy** aplikacji, zobacz Magazyn haseł dla logowania pojedynczego przy użyciu serwera [proxy aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Rozwiązywanie problemów z serwerem proxy** aplikacji: zalecamy rozpoczęcie od przejrzenia przepływu rozwiązywania problemów, debugowania problemów z łącznikiem serwera [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)aplikacji w celu ustalenia, czy łączniki serwera proxy aplikacji są poprawnie skonfigurowane. Jeśli nadal masz problemy z nawiązaniem połączenia z aplikacją, postępuj zgodnie z przepływem rozwiązywania problemów z aplikacją debugowania serwera [proxy aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problemy z [usługą CORS można identyfikować](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) przy użyciu narzędzi debugowania przeglądarki:
    - Uruchom przeglądarkę i przejdź do aplikacji sieci Web.
    - Naciśnij **klawisz F12,** aby przywrócić konsolę debugowania.
    - Spróbuj odtworzyć transakcję i przejrzyj komunikat konsoli. Naruszenie cors powoduje błąd konsoli o pochodzeniu.
    - Niektórych problemów z usługą CORS nie można rozwiązać, na przykład gdy aplikacja przekierowuje do usługi login.microsoft.com w celu uwierzytelnienia, a token dostępu wygasa. Połączenie CORS kończy się niepowodzeniem. Obejściem tego scenariusza jest przedłużenie okresu istnienia tokenu dostępu, aby zapobiec jego wygasaniu w trakcie sesji użytkownika. Aby uzyskać więcej informacji na temat tego, jak to zrobić, zobacz Konfigurowanie okresów istnienia tokenu w [platformie tożsamości firmy Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Rozwiązywanie problemów z logowaniem pojedynczym opartym na programie **SAML:** zalecamy sprawdzenie problemów z logowaniem się do aplikacji skonfigurowanych za pomocą logowania pojedynczego opartego na systemie [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)aby znaleźć rozwiązania problemów, które najprawdopodobniej wystąpią.
5. **Rozwiązywanie problemów z logowaniem** pojedynczym opartym na hasłach: zalecamy sprawdzenie narzędzia do rozwiązywania problemów z logowaniem pojedynczym opartym na hasłach w usłudze [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)aby znaleźć rozwiązania problemów, które najprawdopodobniej wystąpią.
6. Aby uzyskać informacje o problemach z połączeniem podczas korzystania z połączenia VPN, zobacz Jak używać logowania jednokrotnego przez sieć VPN i Wi-Fi [sieci.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
