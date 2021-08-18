---
title: Tworzenie użytkownika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896725"
---
# <a name="create-user"></a>Tworzenie użytkownika

**OGŁOSZENIE:**

- [Od 4 stycznia 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) r. firma Google wyloguje obsługę logowania WebView z usługi Google. Sprawdź, czy na Twoje aplikacje mogą mieć wpływ wskazówki [firmy Google](https://go.microsoft.com/fwlink/?linkid=2157323) dotyczące testowania zgodności.
- Upewnij się, że podczas logowania użytkowników za pomocą kont Google dla klientów indywidualnych używasz systemowego widoku sieci Web lub przeglądarki systemowej. Aby uzyskać więcej informacji, zobacz Problemy z [logowaniem się do aplikacji tylko przy użyciu przeglądarki Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nie mogę utworzyć nowego użytkownika w katalogu usługi Azure AD**

1. Upewnij się, że masz uprawnienia do tworzenia nowego użytkownika standardowego. Nowego użytkownika standardowego może utworzyć tylko administrator globalny Azure Active Directory (AD, User administrator). Jeśli nie pełnisz jednej z tych ról, poproś administratora, aby dodał Cię do jednej z tych ról lub tworzył nowe konto użytkownika dla Ciebie.
1. Upewnij się, że nazwa użytkownika znajduje się w domenie, która została zweryfikowana w usłudze Azure AD. Jeśli w usłudze Azure AD nie ma żadnych zweryfikowanych niestandardowych nazw domen, możesz użyć domeny początkowej usługi Azure AD, która kończy się na *.onmicrosoft.com.
1. Upewnij się, że nazwa użytkownika znajduje się w domenie, która nie jest federowana z usługą Azure AD z lokalnej usługi AD. Użytkowników nie można dodawać w chmurze za pomocą nazw domen, które są federowane ze środowisk lokalnych.
1. Upewnij się, że żaden inny użytkownik lub kontakt nie ma nazwy użytkownika, którą chcesz przypisać noweowi użytkownikowi. Nazwy użytkowników muszą być unikatowe w usłudze Azure AD.
1. Zobacz [Role i administratorzy usługi Azure AD dla](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) usługi Azure AD.
1. Zobacz nazwy [domen dla](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) usługi Azure AD.
1. Przejrzyj [dzienniki inspekcji,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) aby wyświetlić bardziej szczegółowe informacje o ostatnio utworzonym lub usuniętym użytkowniku, na przykład o tym, kto i kiedy wykonał dane działanie.
1. Aby uzyskać więcej informacji na temat dodawania nowych użytkowników, zobacz Tworzenie nowego użytkownika w usłudze Azure AD za pomocą portalu [Azure Portal.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Role administracyjne usługi Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)uprawnienia roli administratora w usłudze Azure Active Directory
1. Możesz również utworzyć nowego użytkownika za pomocą programu [PowerShell usługi Azure AD.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
