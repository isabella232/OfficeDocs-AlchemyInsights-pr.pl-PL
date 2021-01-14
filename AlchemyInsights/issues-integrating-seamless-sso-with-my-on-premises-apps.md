---
title: Problemy z integracją SSO z moimi aplikacjami lokalnymi
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868719"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemy z integracją SSO z moimi aplikacjami lokalnymi

Aby rozwiązać problemy polegające na integrowaniu bezproblemowej rejestracji jednokrotnej z aplikacjami lokalnymi, wykonaj następujące czynności:

**Zalecane kroki**

1. Aby skonfigurować **aplikację lokalną** do rejestracji jednokrotnej **za pośrednictwem serwera proxy aplikacji**, zobacz [magazynowanie haseł w celu rejestracji jednokrotnej za pomocą serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Rozwiązywanie problemów z serwerem proxy aplikacji**: zalecamy rozpoczęcie przeglądu przepływu rozwiązywania problemów oraz [Debugowanie problemów z łącznikiem serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)w celu określenia, czy łączniki serwera proxy aplikacji są skonfigurowane poprawnie. Jeśli nadal występują problemy z połączeniem z aplikacją, postępuj zgodnie z instrukcjami [dotyczącymi rozwiązywania problemów z aplikacją Application proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). [Problemy dotyczące specyfikacji CORS można znaleźć](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) przy użyciu następujących narzędzi debugowania przeglądarki:
    1. Uruchom przeglądarkę i przejdź do aplikacji sieci Web.
    1. Naciśnij klawisz **F12** , aby wywołać konsolę debugowania.
    1. Spróbuj odtworzyć transakcję i przejrzyj komunikat konsoli. Naruszenie specyfikacji CORS powoduje błąd konsoli dotyczącej pochodzeniu.
    1. Nie można rozwiązać kilku problemów dotyczących składnika CORS, takich jak aplikacja przekierowuje do login.microsoftonline.com w celu uwierzytelnienia, a token dostępu wygasa. Nawiązanie połączenia CORS nie powiedzie się. Obejście tego scenariusza polega na przedłużeniu okresu istnienia tokenu dostępu, aby zapobiec wygaśnięciu go podczas sesji użytkownika. Aby uzyskać więcej informacji o tym, jak to zrobić, zobacz [konfigurowalne okresy ważności tokenów na platformie Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Polecane dokumenty**

- [Jak skonfigurować Logowanie jednokrotne w aplikacji proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Logowanie jednokrotne w usłudze SAML dla aplikacji lokalnych z serwerem proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Opis i rozwiązywanie problemów dotyczących proxy aplikacji Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Rozwiązywanie problemów dotyczących konfiguracji delegowania ograniczonego protokołu Kerberos dla serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)