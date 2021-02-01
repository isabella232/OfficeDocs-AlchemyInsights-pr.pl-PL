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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063661"
---
# <a name="configure-and-customize-applications"></a>Konfigurowanie i dostosowywanie aplikacji

**Konfigurowanie aplikacji**

1. Szybki start: Konfigurowanie właściwości aplikacji w dzierżawie usługi [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pokazuje, jak skonfigurować niektóre właściwości aplikacji.
2. Aby ułatwić integrację aplikacji z usługą Azure Active Directory, opracowaliśmy kolekcję [samouczków,](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) które pomogą Ci w konfiguracji.
3. [Sposób konfigurowania aplikacji proxy pomaga](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) zrozumieć, jak skonfigurować aplikację application proxy w usłudze Azure AD w celu udostępnienia aplikacji lokalnych w chmurze.
4. Pobierz program [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)i skonfiguruj aplikację: postępuj zgodnie z instrukcjami w konfigurowaniu programu *PingAccess* dla usługi Azure AD w celu ochrony aplikacji opublikowanych przy użyciu serwera proxy aplikacji usługi Microsoft Azure AD w witrynie internetowej tożsamości ping i pobierz najnowszą wersję programu PingAccess.

**Błędnie skonfigurowana aplikacja (AADSTS650056)**

1. Upewnij się, że uzyskujesz dostęp do aplikacji z adresu logowania podanego przez właściciela aplikacji. W przeciwnym razie zaloguj się do aplikacji w ramach jej zwykłego procesu. W większości przypadków ta funkcja automatycznie rozwiąże problem w sposób naturalny. Jeśli tak się nie stanie, ten wpis może pomóc w rozwiązaniu problemu.
2. **Jeśli Twoja organizacja jest właścicielem aplikacji** (co oznacza, że rejestracja aplikacji jest w Twojej organizacji):
    - Zalecane jest co najmniej dodanie uprawnień `User.Read` lub `openid` uprawnień delegowanych z programu Microsoft **Graph.**
    - Upewnij się, że aplikacja i wszystkie jej uprawnienia są na to zgodę. Możesz to sprawdzić, patrząc na **kolumnę Stan** rejestracji aplikacji w ramach uprawnień **interfejsu API.**
    - W niektórych scenariuszach aplikacja może być aplikacją innej firmy, ale może być zarejestrowana w Twojej organizacji. Potwierdź, czy ta aplikacja znajduje się na liście rejestracji aplikacji (nie aplikacje dla przedsiębiorstw).
    - Jeśli ten komunikat o błędzie będzie nadal wyświetlany. Następnie może być konieczne skompilowanie adresu URL zgody opisanego **w kroku 4.**
3. **Jeśli Twoja organizacja nie jest właścicielem aplikacji i używa jej jako aplikacji innej firmy:**
    - Jeśli jesteś administratorem globalnym/firmowym, powinien zostać wyświetlony ekran zgody. Upewnij się, że jest to pole wyboru **"Zgoda w imieniu Twojej organizacji".**
    - Jeśli nie widzisz ekranu zgody, usuń aplikację Enterprise i spróbuj ponownie.
    - Jeśli ten komunikat o błędzie będzie nadal wyświetlany. Następnie może być konieczne skompilowanie adresu URL zgody opisanego **w kroku 4.**
4. Ręcznie skompilowaj adres **URL** zgody, który ma być używany: Jeśli aplikacja jest przeznaczona do uzyskiwania dostępu do określonego zasobu, używanie przycisków Zgody z portalu Azure Portal może być możliwe, konieczne będzie ręczne wygenerowanie adresu URL zgody i użycie go.
    - Musisz pobrać i `{App-Id}` od `{App-Uri-Id}` właściciela aplikacji. `{Tenant-Id}` będzie Twoim identyfikatorem dzierżawy. Będzie to identyfikator `yourdomain.onmicrosoft.com` katalogu lub identyfikator katalogu.
    - Jeśli aplikacja uzyskuje dostęp do samej zasobu, to i `{App-Id}` `{App-Uri-Id}` będzie taki sam.
5. Aby uzyskać więcej informacji, zobacz Problemy z logowaniem się do aplikacji skonfigurowanych do logowania się pojedynczego opartego na [forach SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Dostosowywanie aplikacji**

- Dodaj znakowanie do strony logowania w usłudze [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) swojej organizacji — użyj logo i niestandardowych schematów kolorów swojej organizacji, aby zapewnić spójny wygląd i sposób działania na stronach logowania usługi Azure Active Directory (Azure AD).
- [Dodaj niestandardową nazwę domeny za pomocą portalu usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) — każda nowa dzierżawa usługi Azure AD zawiera początkową nazwę domeny. Nie można zmienić ani usunąć początkowej nazwy domeny, ale można dodać nazwy organizacji. Dodawanie niestandardowych nazw domen ułatwia tworzenie nazw użytkowników znanych użytkownikom.
