---
title: Konfigurowanie bezproblemowego logowania jednokrotnego
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841533"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurowanie bezproblemowego logowania jednokrotnego

**Konfigurowanie aplikacji**

1. Należy pobrać wartości od dostawcy aplikacji. Możesz ręcznie wprowadzić wartości lub przekazać plik metadanych w celu wyodrębnienia wartości pól.
2. Wiele aplikacji zostało już wstępnie skonfigurowanych do współpracy z usługą Azure AD. Te aplikacje są wymienione w galerii aplikacji, które można przeglądać podczas dodawania aplikacji do dzierżawy usługi Azure AD. Seria [Szybki start](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) umożliwia ten proces.
3. Aby utworzyć aplikację, która nie jest galerią, kliknij przycisk **+ Utwórz** własną aplikację i nadaj nazwę aplikacji.
    - Domyślnie wybierze opcję Integruj **każdą** inną aplikację, której nie ma w galerii, co jest właściwą opcją w aplikacjach niebędąca galerią.
    - Po umieszczeniu **nazwy aplikacji** na stronie Utwórz utworzy ona nową aplikację bez galerii dla przedsiębiorstw.
    - Następnie możesz przejść do logowania **pojedynczego** w obszarze Zarządzanie aplikacją, aby zobaczyć różne techniki implementowania go w środowisku. 

**Konfigurowanie bezproblemowego logowania jednokrotnego dla określonej aplikacji**

Szczegółowe instrukcje krok po kroku znajdziesz w galerii aplikacji. Aby uzyskać dostęp do tych czynności, możesz przejrzeć listę wszystkich samouczków konfiguracji aplikacji dostępnych w samouczkach konfiguracji [aplikacji SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurowanie logowania jednokrotnego opartego na programie SAML**

1. Szybki start: konfigurowanie logowania jednokrotnego [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)opartego na wersji SAML dla aplikacji w dzierżawie usługi Azure Active Directory (Azure AD).
2. Aby dowiedzieć się więcej o opcji logowania pojedynczego opartego na językach SAML, zobacz Opis logowania pojedynczego opartego na programie [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Aby dowiedzieć się więcej o żądaniach uwierzytelniania w wersji 2.0 SAML i odpowiedziach, które obsługuje usługa Azure Active Directory (Azure AD) dla logowania jednokrotnego (SSO), zobacz Protokół SINGLE Sign-On [Sign-On SAML.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Aby dowiedzieć się, jak tworzyć i konfigurować logowanie jednokrotne oparte na technologii SAML dla aplikacji w usłudze Azure Active Directory (Azure AD) przy użyciu interfejsu API Microsoft Graph, zobacz Konfigurowanie logowania jednokrotnego opartego na programie SAML dla aplikacji przy użyciu interfejsu [API Microsoft Graph.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Aby dowiedzieć się, jak usługa Azure AD używa protokołu SAML, zobacz W jaki sposób [platforma tożsamości firmy Microsoft używa protokołu SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurowanie tokenów i roszczeń**

1. [Jak dostosować roszczenia wydane w tokenie SAML dla aplikacji dla przedsiębiorstw.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Aby dowiedzieć się, jak konfigurować roszczenia przy użyciu programu PowerShell, zobacz Jak to zrobić: Dostosowywanie roszczeń pominiętych w tokenach dla określonej aplikacji w dzierżawie [(wersja Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Aby dowiedzieć się, jak skonfigurować opcjonalne roszczenia, zobacz Jak: zapewnianie opcjonalnych [roszczeń dla aplikacji.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Aby dowiedzieć się, jak używać atrybutów rozszerzenia schematu katalogu w celu wysyłania danych użytkowników do aplikacji w oświadczeniach tokenu, zobacz Używanie atrybutów rozszerzenia schematu [katalogu w oświadczeniach.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Aby dowiedzieć się, jak skonfigurować okresy istnienia tokenu, zobacz Konfigurowanie okresów istnienia [tokenu w platformie tożsamości Microsoft (wersja Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. Konfigurowanie zasad cyklu życia tokenu [(wersja Zapoznawcza)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) — w tym artykule omykamy typowe scenariusze zasad, które mogą ułatwić nakładanie nowych reguł na okres istnienia tokenu. W tym przykładzie dowiesz się, jak utworzyć zasady wymagające, aby użytkownicy częściej uwierzytelniali się w aplikacji sieci Web.

**Rozwiązywanie problemów z konfiguracją logowania jednokrotnego**

- Aby uzyskać odpowiedzi na często zadawane pytania dotyczące bezproblemowego logowania jednokrotnego w usłudze Azure Active Directory Sign-On (bezproblemowe logowanie jednokrotne), zobacz Bezproblemowe logowanie jednokrotne w usłudze [Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)często zadawane pytania.
- Aby uzyskać informacje na temat rozwiązywania typowych problemów związanych z bezproblemowym logowaniem jednokrotnym w usłudze Azure Active Directory (Azure AD Sign-On), zobacz Rozwiązywanie problemów z bezproblemowym logowaniem jednokrotnym w usłudze [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
