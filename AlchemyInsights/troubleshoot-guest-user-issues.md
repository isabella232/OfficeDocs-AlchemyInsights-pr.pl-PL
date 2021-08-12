---
title: Rozwiązywanie problemów z użytkownikiem gości
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939389"
---
# <a name="troubleshoot-guest-user-issues"></a>Rozwiązywanie problemów z użytkownikiem gości

1. Aby uzyskać wskazówki na temat zarządzania dostępem gości do aplikacji, zobacz Zarządzanie dostępem gościa [za pomocą recenzji dostępu](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)do usługi Azure AD.
1. Dodawanie użytkowników gości do katalogu w portalu [Azure Portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)W ramach tego przewodnika Szybki start dodasz nowego gościa do katalogu usługi Azure AD za pośrednictwem portalu Azure Portal, wyślesz zaproszenie i zobaczysz, jak wygląda proces realizacji zaproszenia użytkownika gościa.
1. [Dodaj gościa za pomocą programu PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)W tym przewodniku Szybki start użyjesz New-AzureADMSInvitation, aby dodać jednego gościa do dzierżawy platformy Azure.
1. Aby dowiedzieć się, jak przypisywać użytkowników i grupy do aplikacji dla przedsiębiorstw w usłudze Azure Active Directory (Azure AD), z poziomu portalu Azure lub przy użyciu programu PowerShell, zobacz Zarządzanie przypisaniem użytkowników do aplikacji w usłudze [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory B2B (Azure AD) współpracuje z większość aplikacji integrują się z usługą Azure AD. W tym [artykule](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)omymy się z instrukcjami dotyczącymi konfigurowania niektórych popularnych aplikacji SaaS do używania z usługą Azure AD B2B.
1. Jako organizacja, która używa funkcji współpracy B2B usługi Azure Active Directory (Azure AD) w celu zapraszania użytkowników gości z organizacji partnerskich do usługi Azure AD, możesz teraz udostępnić tym użytkownikom B2B dostęp do aplikacji lokalnych. Te aplikacje lokalne mogą korzystać z uwierzytelniania opartego na protokołu SAML lub zintegrowanego uwierzytelniania sieci Windows (IWA) z delegowaniem ograniczonym Kerberos (KCD). Aby uzyskać więcej informacji, zobacz Udzielanie użytkownikom [B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)dostępu do aplikacji lokalnych w usłudze Azure AD.
1. Dowiedz się, jak [udzielić kontom partnerów](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)zarządzanych lokalnie dostępu do zasobów w chmurze przy użyciu funkcji współpracy B2B usługi Azure AD.