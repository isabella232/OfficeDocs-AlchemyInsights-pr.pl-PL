---
title: Problemy z oświadczeniami i atrybutami tokenu
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012894"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemy z oświadczeniami i atrybutami tokenu

**Aktualizowanie, konfigurowanie lub usuwanie roszczeń tokenu**

1. Za pomocą Azure Active Directory (Azure AD) możesz dostosować typ [żądania](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) dla żądania roli w tokenie odpowiedzi, który otrzymasz po autoryzowaniu aplikacji.
2. Deweloperzy aplikacji mogą używać opcjonalnych roszczeń w swoich aplikacjach usługi Azure AD, aby określić, które roszczenia chcą mieć w tokenach wysłanych do swoich aplikacji. Aby uzyskać więcej informacji, [zobacz Zapewnianie opcjonalnych roszczeń dotyczących aplikacji.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurowanie roszczeń grupy dla aplikacji z Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. W przypadku korzystania z bezproblemowego logowania pojedynczego w aplikacji zobacz Dostosowywanie roszczeń wydanych w [tokenie SAML dla aplikacji dla przedsiębiorstw.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapowanie atrybutów roszczeń**

1. Aby skonfigurować zasady mapowania roszczeń przy użyciu programu PowerShell, zobacz Dostosowywanie roszczeń pominiętych w tokenach dla określonej aplikacji w dzierżawie [(wersja Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atrybuty rozszerzenia schematu katalogu zapewniają sposób przechowywania dodatkowych danych w Azure Active Directory obiektach użytkowników i innych obiektach katalogu, takich jak grupy, szczegóły dzierżawy czy podmioty zabezpieczeń usług. Do emitowania roszczeń wobec aplikacji można używać tylko atrybutów rozszerzenia obiektów użytkownika. [Używanie atrybutów rozszerzenia schematu katalogu w oświadczeniach](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) opisuje sposób korzystania z atrybutów rozszerzenia schematu katalogu w celu wysyłania danych użytkowników do aplikacji w oświadczeniach tokenu.

Aby uzyskać więcej informacji na temat roszczeń tokenu, zobacz:

- [Roszczenia w tokenach dostępu](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Roszczenia w id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C
- [Odwołanie do roszczeń tokenu SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
