---
title: Problemy dotyczące właściciela rejestracji aplikacji
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404780"
---
# <a name="app-registration-owner-issues"></a>Problemy dotyczące właściciela rejestracji aplikacji

Poniżej przedstawiono dostępne metody dodawania podmiotów głównych jako właścicieli rejestracji aplikacji:

- Moduł PowerShell usługi Azure AD —

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Informacje: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Korzystanie z funkcji Azure CLI — `az ad app owner add`

    Informacje: [właściciel aplikacji az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Używanie funkcji MS Graph —

    Informacje: [Dodawanie właściciela — Microsoft Graph w wersji 1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Korzystanie z portalu usługi Azure AD — przejdź do portal.azure.com [>](https://portal.azure.com/) usługi Azure Active Directory > rejestracja aplikacji > Wybierz aplikację > Właściciele > Dodaj właścicieli

**Nie możesz wyświetlić aplikacji na tablicy rejestracji aplikacji, nawet jeśli jesteś właścicielem tej aplikacji?**

Właściciel aplikacji nie jest rolą administracyjną. Jeśli ustawienie Ogranicz dostęp do portalu administracyjnego [usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) jest włączone, tylko administrator będzie mógł wyświetlać aplikacje w portalu rejestracji aplikacji. Aby właściciel mógł wyświetlać aplikacje, wyłącz to ustawienie (Ustaw to na wartość NIE) lub przypisz rolę administratora tylko do konkretnej aplikacji. Jednak w tym celu należy wymagać licencji Azure AD Premium P2 i włączyć [zarządzanie tożsamością privileged.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
