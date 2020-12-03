---
title: Usuwanie dzierżawy
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564885"
---
# <a name="delete-tenant"></a>Usuwanie dzierżawy

Aby usunąć usługę Azure AD, upewnij się, że:
- Jesteś administratorem globalnym w katalogu.
- Użytkownik nie jest zalogowany przy użyciu konta, które ma katalog domyślny, taki jak contoso.onmicrosoft.com na koncie zalogowanym, na przykład admin@contoso.onmicrosoft.com.
- Przed usunięciem Usuń wszystkie aktywne aplikacje w katalogu. Aby usunąć aktywne aplikacje, przejdź do rejestracji aplikacji i Usuń istniejące aplikacje.
- Nie ma aktywnych subskrypcji żadnych usług Microsoft Online, takich jak Microsoft Azure, Office 365 lub Azure AD Premium, które są skojarzone z katalogiem. Przekazywanie abonamentów lub przyspieszanie anulowania aktywnych subskrypcji za pośrednictwem usługi Azure support i rozliczenia. Dowiedz się więcej o tym, jak anulować subskrypcję usługi Office 365 i subskrypcje platformy Azure. Aby uzyskać wskazówki dotyczące kojarzenia lub dodawania istniejącej subskrypcji do dzierżawy, zobacz [kojarzenie lub Dodawanie subskrypcji platformy Azure do dzierżawy usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Brak aktywnych licencji. Aby usunąć licencje, zobacz [Jak usunąć subskrypcję w celu usunięcia licencji](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Po próbie usunięcia usługi Azure AD nie ma żadnych innych aktywnych użytkowników w katalogu, ani jako Administrator globalny. Usuń wszystkich innych aktywnych użytkowników, a wszystkie zależności dotyczące niestandardowej nazwy domeny w dzierżawie również muszą zostać usunięte, na przykład użytkownicy utworzeni za pomocą admin@contoso.com.

Aby uzyskać więcej szczegółowych informacji na temat następujących czynności:
- Usuń usługę Azure Active Directory lub "abonament", zobacz [usuwanie usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Usuwanie aplikacji w katalogu, zobacz [usuwanie aplikacji](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
