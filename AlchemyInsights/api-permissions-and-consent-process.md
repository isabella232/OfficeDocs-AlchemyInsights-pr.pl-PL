---
title: Proces uprawnień i zgody interfejsu API
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404876"
---
# <a name="api-permissions-and-consent-process"></a>Proces uprawnień i zgody interfejsu API

Aby Twoja aplikacja uzyskać dostęp do danych w programie Microsoft Graph, użytkownik lub administrator musi udzielić im właściwych uprawnień w ramach procesu zgody. [W odwołani do uprawnień programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) wymieniono uprawnienia skojarzone z każdym głównym zestawem interfejsów API programu Microsoft Graph. Zawiera również wskazówki dotyczące korzystania z tych uprawnień.

**Konfigurowanie lub aktualizowanie podmiotu zabezpieczeń usługi**

- [Tworzenie właściwości serviceprincipal —](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) w tym artykule pokazano, jak utworzyć nowy obiekt servicePrincipal.
- Tworzenie podmiotu zabezpieczeń [usługi Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) w portalu — w tym artykule pokazano, jak utworzyć nową aplikację i podmiot zabezpieczeń usługi Azure Active Directory (Azure AD), których można używać z kontrolką dostępu opartą na rolach.
- [Aplikacje &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) głównych użytkowników usługi w usłudze Azure AD — w tym artykule opisano rejestrację aplikacji, obiekty aplikacji i podmioty zabezpieczeń usług w usłudze Azure Active Directory: co to są, jak są używane i jak są powiązane ze sobą.

**Dodawanie lub aktualizowanie rejestracji aplikacji i wyrażanie zgody administratora**

- [Tworzenie rejestracji aplikacji —](https://docs.microsoft.com/graph/api/application-post-applications) w tym artykule pokazano, jak utworzyć nowy obiekt aplikacji.
- [Aktualizowanie rejestracji aplikacji — uprawnienia interfejsu API](https://docs.microsoft.com/graph/api/application-update) — w tym artykule pokazano, jak zaktualizować właściwości obiektu aplikacji.
- [Zapewnij zgodę administratora](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) — aby uzyskać zgodę administratora, na ogół wymagamy wyrażenia zgody przez administratora.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) — kontener zarządzania rolami dla ujednoliconych definicji ról i przydziałów ról dla dostawców RBAC platformy Microsoft 365, którzy obsługują wiele głównych użytkowników i wiele zakresów w jednym przypisaniu ról. To inny niż *typ zasobu rbacApplication.* Przykładem takiego dostawcy RBAC jest usługa Microsoft Intune. Przypisanie roli w usłudze Intune może mieć tablicę głównych użytkowników i szereg grup zakresów. **Jest to wersja beta, co oznacza, że jest ona nadal w fazie opracowywania i nie jest zalecana do użycia w środowisku produkcyjnym.**
