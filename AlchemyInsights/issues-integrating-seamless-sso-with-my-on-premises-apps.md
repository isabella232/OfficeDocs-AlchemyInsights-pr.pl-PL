---
title: Problemy ze zintegrowaniem bezproblemowego logowania jednokrotnego z aplikacjami lokalnymi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028302"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemy ze zintegrowaniem bezproblemowego logowania jednokrotnego z aplikacjami lokalnymi

Aby rozwiązać problemy dotyczące integrowania bezproblemowego logowania jednokrotnego z aplikacjami lokalnymi, wykonaj następujące czynności:

**Zalecane czynności**

1. Aby skonfigurować aplikację **lokalną do** logowania pojedynczego za pośrednictwem serwera **proxy** aplikacji, zobacz Magazyn haseł dla logowania pojedynczego przy [użyciu application proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Rozwiązywanie problemów z serwerem proxy** aplikacji: zalecamy rozpoczęcie od przejrzenia przepływu rozwiązywania problemów, [debugowania](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemów z łącznikiem serwera proxy aplikacji , w celu ustalenia, czy łączniki serwera proxy aplikacji są poprawnie skonfigurowane. Jeśli nadal masz problemy z nawiązaniem połączenia z aplikacją, postępuj zgodnie z instrukcjami rozwiązywania problemów z [aplikacją debugowania](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)proxy. Problemy z [usługą CORS można zidentyfikować,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) korzystając z następujących narzędzi do debugowania w przeglądarce:
    1. Uruchom przeglądarkę i przejdź do aplikacji sieci Web.
    1. Naciśnij **klawisz F12,** aby przywrócić konsolę debugowania.
    1. Spróbuj odtworzyć transakcję i przejrzeć komunikat konsoli. Naruszenie corsu powoduje błąd konsoli o pochodzeniu.
    1. Niektórych problemów z usługą CORS nie można rozwiązać, na przykład gdy aplikacja przekierowuje do usługi login.microsoftonline.com w celu uwierzytelnienia i token dostępu wygasa. Połączenie CORS kończy się niepowodzeniem. Obejściem tego scenariusza jest przedłużenie okresu istnienia tokenu dostępu, aby zapobiec jego wygaśnięciu w trakcie sesji użytkownika. Aby uzyskać więcej informacji na ten temat, zobacz Konfigurowanie okresów istnienia tokenu w [programie Platforma tożsamości Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Polecane dokumenty**

- [Jak skonfigurować logowanie pojedyncze do aplikacji application proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Logowanie pojedyncze SAML dla aplikacji lokalnych z serwerem proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Opis i rozwiązywanie Azure Active Directory cors serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Rozwiązywanie problemów z konfiguracjami delegowania ograniczonego protokołu Kerberos dla serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)