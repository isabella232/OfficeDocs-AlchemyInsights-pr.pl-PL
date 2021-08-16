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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028086"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemy z podmiotem zabezpieczeń zasobu lub usługi

1. Jeśli dopiero zaczynasz pracę, obiekty główne aplikacji i usług w programie [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) opisują rejestrację aplikacji, obiekty aplikacji i podmioty zabezpieczeń usług w programie Azure Active Directory: ich opis, sposób ich stosowania i sposób ich powiązania. Przedstawiony jest również scenariusz przykładowy dla wielu dzierżaw, który przedstawia relację między obiektem aplikacji aplikacji a odpowiadającymi im obiektami głównymi usługi.
2. Aby dowiedzieć się więcej o relacji między aplikacjami a podmiotami zabezpieczeń usługi, zobacz aplikacje i obiekty podmiotu zabezpieczeń usługi w [programie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Jak to zrobić: Za pomocą portalu można utworzyć podmiot zabezpieczeń aplikacji i usługi [Azure AD,](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) który może uzyskać dostęp do zasobów, aby dowiedzieć się, jak utworzyć nową aplikację i podmiot zabezpieczeń usługi Azure Active Directory (Azure AD), który może być używany z kontrolką dostępu opartą na rolach.
4. Za pomocą [interfejsu API podmiotu](https://docs.microsoft.com/graph/api/resources/serviceprincipal)zabezpieczeń usługi możesz programowo zarządzać wystąpieniami aplikacji i kontrolować, co aplikacja może robić w ramach Twojej dzierżawy.
5. [Typ zasobu servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) zawiera listę wszystkich właściwości i metod dla typu zasobu servicePrincipal.
6. [Różnice między typami zasobów](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) między usługą Azure AD Graph a usługą Microsoft Graph podkreślono różnice między usługami Azure AD Graph i Microsoft Graph zasobów. Przedstawia on zasoby, które mają różne nazwy lub są niedostępne. Wyróżniane są również zasoby dostępne w wersji beta pakietu Microsoft Graph ale nie w wersji 1.0.

**Problemy z użytkownikami-gośćmi**

- [Szybki start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Dodaj użytkowników gości do katalogu w portalu Azure Portal, aby dowiedzieć się, jak dodać nowego gościa do katalogu usługi Azure AD za pośrednictwem portalu Azure Portal, wysłać zaproszenie i zobaczyć, jak wygląda proces realizacji zaproszenia użytkownika gościa.
- [Samouczek: Utwórz przepływy użytkownika w Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) pokazano, jak utworzyć kilka zalecanych przepływów użytkownika przy użyciu portalu Azure Portal. Jeśli szukasz informacji na temat konfigurowania przepływu poświadczeń hasła właściciela zasobu w aplikacji, zobacz Konfigurowanie przepływu poświadczeń hasła właściciela zasobu w usłudze Azure AD B2C.
