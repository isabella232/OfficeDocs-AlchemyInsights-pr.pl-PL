---
title: Konfigurowanie i dostosowywanie aplikacji
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044998"
---
# <a name="configure-and-customize-applications"></a>Konfigurowanie i dostosowywanie aplikacji

**Konfigurowanie aplikacji**

1. Szybki start: Skonfiguruj właściwości aplikacji w dzierżawie usługi [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) aby dowiedzieć się, jak skonfigurować niektóre właściwości aplikacji.
2. Aby ułatwić integrację aplikacji z programem Azure Active Directory, opracowaliśmy kolekcję [samouczków,](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) które pomogą Ci w konfiguracji.
3. [Sposób konfigurowania aplikacji proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) pomaga zrozumieć, jak skonfigurować aplikację proxy aplikacji w usłudze Azure AD w celu udostępnienia aplikacji lokalnych do chmury.
4. Pobierz program [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)i skonfiguruj aplikację: Postępuj zgodnie z instrukcjami w tece Konfigurowanie programu *PingAccess* dla usługi Azure AD w celu ochrony aplikacji opublikowanych przy użyciu serwera proxy aplikacji Microsoft Azure AD w witrynie internetowej tożsamości ping i pobierz najnowszą wersję programu PingAccess.

**Błędnie skonfigurowane aplikacje (AADSTS650056)**

1. Upewnij się, że uzyskujesz dostęp do aplikacji z adresu logowania podanego przez właściciela aplikacji. W przeciwnym razie zaloguj się do aplikacji zgodnie z jej normalnym procesem. W większości przypadków jest to automatyczne rozwiązywanie problemu w sposób naturalny. Jeśli tak się nie stanie, ten wpis może pomóc w rozwiązaniu problemu i jego rozwiązaniu.
2. **Jeśli Twoja organizacja jest właścicielem aplikacji** (co oznacza, że rejestracja aplikacji należy do Twojej organizacji):
    - Zalecane jest co najmniej uprawnienie firmy Microsoft lub uprawnienie delegowane z Graph `User.Read` `openid` Microsoft. 
    - Upewnij się, że aplikacja i wszystkie jej uprawnienia są na to zgodę. Możesz to sprawdzić, patrząc na kolumnę **Stan** w kolumnie Rejestracja aplikacji w ramach uprawnień **interfejsu API.**
    - W niektórych scenariuszach aplikacja może być też aplikacją innej firmy, ale może być zarejestrowana w Twojej organizacji. Potwierdź, czy ta aplikacja znajduje się na liście rejestracji aplikacji (nie dotyczy Enterprise aplikacji).
    - Jeśli ten komunikat o błędzie będzie nadal wyświetlany. W takiej przypadku może być konieczne skompilowanie adresu URL zgody opisanego **w kroku 4.**
3. **Jeśli Twoja organizacja nie jest właścicielem aplikacji i używa jej jako aplikacji innej firmy:**
    - Jeśli jesteś administratorem globalnym/firmowym, powinien zostać wyświetlony ekran zgody. Upewnij się, że jest pole **wyboru "Zgoda w imieniu Twojej organizacji".**
    - Jeśli nie widzisz ekranu zgody, usuń aplikację Enterprise i spróbuj ponownie.
    - Jeśli ten komunikat o błędzie będzie nadal wyświetlany. W takiej przypadku może być konieczne skompilowanie adresu URL zgody opisanego **w kroku 4.**
4. **Ręcznie** skompilowaj adres URL zgody, który ma być używany: Jeśli aplikacja jest przeznaczona do uzyskiwania dostępu do określonego zasobu, możesz nie mieć możliwości używania przycisków Zgody z portalu Azure Portal, musisz ręcznie wygenerować adres URL zgody i użyć go.
    - Musisz pobrać i `{App-Id}` od `{App-Uri-Id}` właściciela aplikacji. `{Tenant-Id}` będzie Twoim identyfikatorem dzierżawy. Będzie to identyfikator `yourdomain.onmicrosoft.com` katalogu.
    - Jeśli aplikacja uzyskuje dostęp do samej zasobu, wówczas `{App-Id}` i `{App-Uri-Id}` będą takie same.
5. Aby uzyskać więcej informacji, zobacz Problemy z logowaniem się do aplikacji skonfigurowanych do logowania się pojedynczego opartego na forach [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Dostosowywanie aplikacji**

- [](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) Dodawanie marki do strony logowania w usłudze Azure Active Directory organizacji — korzystaj z logo i niestandardowych schematów kolorów swojej organizacji, aby zapewnić spójny wygląd i sposób logowania do stron logowania usługi Azure Active Directory (Azure AD).
- [Dodaj niestandardową nazwę domeny za pomocą portalu Azure Active Directory —](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) każda nowa dzierżawa usługi Azure AD jest wyposażona w początkową nazwę domeny. Nie można zmienić ani usunąć początkowej nazwy domeny, ale można dodać nazwy organizacji. Dodawanie niestandardowych nazw domen ułatwia tworzenie nazw użytkowników znanych użytkownikom.
