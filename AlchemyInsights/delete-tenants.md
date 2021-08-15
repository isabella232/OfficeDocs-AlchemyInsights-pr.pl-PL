---
title: Usuń dzierżawę
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993903"
---
# <a name="delete-tenant"></a>Usuń dzierżawę

Aby usunąć usługę Azure AD, upewnij się, że:
- Jesteś administratorem globalnym katalogu.
- UŻYTKOWNIK NIE jest zalogowany przy użyciu konta z katalogiem domyślnym, takim contoso.onmicrosoft.com się na zalogowanym koncie, takim jak konto admin@contoso.onmicrosoft.com.
- Przed usunięciem usuń wszystkie aktywne aplikacje z katalogu. Aby usunąć aktywne aplikacje, przejdź do rejestracji aplikacji i usuń istniejące aplikacje.
- Nie ma aktywnych subskrypcji dla jakichkolwiek usług Online Services firmy Microsoft, takich Microsoft Azure, Office 365 lub Azure AD — wersja Premium skojarzonych z katalogiem. Przekieruj swoje subskrypcje lub przyspiesz anulowanie aktywnych subskrypcji za pośrednictwem pomocy technicznej i rozliczeń platformy Azure. Dowiedz się więcej na temat Office 365 subskrypcji usługi Azure i subskrypcji usługi Azure. Aby uzyskać wskazówki dotyczące kojarzenia lub dodawania istniejącej subskrypcji do dzierżawy, zobacz Kojarzenie lub dodawanie subskrypcji platformy Azure do [dzierżawy usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nie ma aktywnej licencji. Aby usunąć licencje, zobacz [Jak usunąć subskrypcję, aby usunąć licencję.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Oprócz Ciebie jako administratora globalnego podczas próby usunięcia usługi Azure AD w katalogu nie ma żadnych innych aktywnych użytkowników. Usuń wszystkich innych aktywnych użytkowników, a wszelkie zależności od nazwy domeny niestandardowej w dzierżawie także muszą zostać usunięte, na przykład użytkownicy utworzeni za pomocą usługi admin@contoso.com.

Aby uzyskać więcej szczegółowych informacji na temat tego, jak to zrobić:
- Usuń "Azure Active Directory" lub "subskrypcja", zobacz [Usuwanie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Aby usunąć aplikacje z katalogu, zobacz [Usuwanie aplikacji.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
