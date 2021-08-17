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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084356"
---
# <a name="sso-connection-issues"></a>Problemy z połączeniem logowania jednokrotnego

1. Postępuj zgodnie [z oknie Szybki start: konfigurowanie](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) właściwości przewodnika aplikacji w celu skonfigurowania aplikacji.
2. W zależności od wybranej aplikacji i opcji [logowania pojedynczego](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) postępuj zgodnie z poniższymi wskazówkami:
    - Aby skonfigurować aplikację **lokalną dla** logowania pojedynczego opartego na programie **SAML,** zobacz Logowanie pojedyncze SAML dla aplikacji lokalnych z serwerem [proxy aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Aby skonfigurować aplikację **w chmurze** do **logowania** pojedynczego opartego na hasłach, zobacz [Konfigurowanie logowania pojedynczego hasła.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Aby skonfigurować aplikację **lokalną do** logowania pojedynczego za pośrednictwem serwera **proxy** aplikacji, zobacz Magazyn haseł dla logowania pojedynczego przy [użyciu application proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Rozwiązywanie problemów z serwerem proxy** aplikacji: zalecamy rozpoczęcie od przejrzenia przepływu rozwiązywania problemów, [debugowania](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemów z łącznikiem serwera proxy aplikacji , aby sprawdzić, czy łączniki proxy aplikacji są poprawnie skonfigurowane. Jeśli nadal masz problemy z nawiązaniem połączenia z aplikacją, postępuj zgodnie z pływem rozwiązywania problemów z aplikacją [proxy debugowania.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problemy z [usługą CORS można zidentyfikować](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) przy użyciu narzędzi do debugowania przeglądarki:
    - Uruchom przeglądarkę i przejdź do aplikacji sieci Web.
    - Naciśnij **klawisz F12,** aby przywrócić konsolę debugowania.
    - Spróbuj odtworzyć transakcję i przejrzeć komunikat konsoli. Naruszenie corsu powoduje błąd konsoli o pochodzeniu.
    - Niektórych problemów z usługą CORS nie można rozwiązać, na przykład gdy aplikacja przekierowuje do usługi login.microsoft.com w celu uwierzytelnienia, a token dostępu wygasa. Połączenie CORS kończy się niepowodzeniem. Obejściem tego scenariusza jest przedłużenie okresu istnienia tokenu dostępu, aby zapobiec jego wygaśnięciu w trakcie sesji użytkownika. Aby uzyskać więcej informacji na ten temat, zobacz Konfigurowanie okresów istnienia tokenu w [programie Platforma tożsamości Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Rozwiązywanie problemów związanych z logowaniem pojedynczym opartym na programie **SAML:** zalecamy sprawdzenie problemów z logowaniem się do aplikacji skonfigurowanych do logowania pojedynczego opartego na programie [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)aby znaleźć rozwiązania problemów, które najprawdopodobniej wystąpią.
5. **Rozwiązywanie problemów z logowaniem** pojedynczym opartym na hasłach: zalecamy skorzystanie z tematu Rozwiązywanie problemów związanych z logowaniem pojedynczym opartym na hasłach w usłudze [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)aby znaleźć rozwiązania problemów, które najprawdopodobniej wystąpią.
6. Aby uzyskać informacje o problemach z połączeniem podczas korzystania z połączenia VPN, zobacz Jak korzystać z logowania jednokrotnego [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)przez sieć VPN Wi-Fi sieci.
