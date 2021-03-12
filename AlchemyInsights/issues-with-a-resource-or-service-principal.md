---
title: Problemy z podmiotem zabezpieczeń zasobu lub usługi
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714081"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemy z podmiotem zabezpieczeń zasobu lub usługi

1. Jeśli dopiero zaczynasz pracę, obiekty główne aplikacji i usług w usłudze [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) opisują rejestrację aplikacji, obiekty aplikacji i podmioty zabezpieczeń usług w usłudze Azure Active Directory: ich opis, sposób ich stosowania i sposób ich powiązania. Przedstawiony jest również przykładowy scenariusz dla wielu dzierżaw, ilustrujący relację między obiektem aplikacji a odpowiadającymi im obiektami głównymi usługi.
2. Aby dowiedzieć się więcej na temat relacji między aplikacjami i podmiotami zabezpieczeń usługi, przeczytaj informacje o aplikacjach i obiektach głównych usług [w usłudze Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Jak to zrobić: Za pomocą portalu możesz utworzyć podmiot zabezpieczeń aplikacji i usług [Azure AD,](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) który może uzyskać dostęp do zasobów, aby dowiedzieć się, jak utworzyć nową aplikację i podmiot zabezpieczeń usługi Azure Active Directory (Azure AD), która może być używana razem z kontrolką dostępu opartą na rolach.
4. Za pomocą [interfejsu API podmiotu zabezpieczeń](https://docs.microsoft.com/graph/api/resources/serviceprincipal)usługi możesz programowo zarządzać wystąpieniami aplikacji i kontrolować, co aplikacja może robić w ramach Twojej dzierżawy.
5. [Typ zasobu servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) zawiera listę wszystkich właściwości i metod dla typu zasobu ServicePrincipal.
6. [Różnice między typami zasobów między programem Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) a programem Microsoft Graph podkreślają różnice między zasobami programu Azure AD Graph i programu Microsoft Graph. Przedstawia zasoby o różnych nazwach lub niedostępne. Ponadto wyróżniane są zasoby dostępne w wersji beta programu Microsoft Graph, ale nie w wersji 1.0.

**Problemy z użytkownikami gośćmi**

- [Szybki start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Dodaj użytkowników gości do katalogu w portalu Azure Portal, aby dowiedzieć się, jak dodać nowego użytkownika gościa do katalogu usługi Azure AD za pośrednictwem portalu Azure Portal, wysłać zaproszenie i zobaczyć, jak wygląda proces realizacji zaproszenia użytkownika gościa.
- [Samouczek: Tworzenie przepływów użytkowników w centrum B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) usługi Azure Active Directory pokazuje, jak tworzyć zalecane przepływy użytkowników za pomocą portalu Azure Portal. Jeśli szukasz informacji na temat konfigurowania przepływu poświadczeń hasła właściciela zasobu w aplikacji, zobacz Konfigurowanie przepływu poświadczeń hasła właściciela zasobu w usłudze Azure AD B2C.
