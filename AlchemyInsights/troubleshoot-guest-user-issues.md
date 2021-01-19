---
title: Rozwiązywanie problemów z użytkownikami Gości
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901585"
---
# <a name="troubleshoot-guest-user-issues"></a>Rozwiązywanie problemów z użytkownikami Gości

1. Aby uzyskać wskazówki dotyczące zarządzania dostępem Gości do aplikacji, zobacz [Zarządzanie dostępem gościa za pomocą recenzji usługi Azure AD Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Dodaj użytkowników będących gośćmi do katalogu w portalu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): w tym szybkim uruchomieniu dodasz nowego użytkownika będącego gościem do katalogu usługi Azure AD za pośrednictwem portalu Azure, Wyślij zaproszenie i zobacz, co wygląda na proces realizacji zaproszeń użytkownika będącego gościem.
1. [Dodawanie użytkownika będącego gościem za pomocą programu PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): w tym szybkim uruchomieniu użyj polecenia New-AzureADMSInvitation, aby dodać jednego użytkownika będącego gościem do dzierżawy usługi Azure.
1. Aby dowiedzieć się, jak przypisywać użytkowników i grupy do aplikacji dla przedsiębiorstw w usłudze Azure Active Directory (Azure AD), w witrynie Azure Active Directory lub za pomocą programu PowerShell zobacz [Zarządzanie przypisaniem przez użytkownika aplikacji w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Współpraca za pomocą usługi Azure Active Directory (Azure AD) działa w przypadku większości aplikacji integrujących się z usługą Azure AD. W tym [artykule](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)omówiono instrukcje dotyczące konfigurowania kilku popularnych aplikacji SaaS do użytku z usługą Azure AD B2B.
1. Jako organizacja korzystająca z funkcji współpracy w usłudze Azure Active Directory (Azure AD) do zapraszania użytkowników będących gośćmi z organizacji partnerskich do usługi Azure AD, możesz teraz udostępnić tych użytkownikom programu B2B dostęp do aplikacji lokalnych. Te aplikacje lokalne mogą korzystać z uwierzytelniania opartego na protokole SAML lub zintegrowanego uwierzytelniania systemu Windows (IWA) za pomocą ograniczonego delegowania Kerberos (KCD). Aby uzyskać więcej informacji, zobacz [udzielanie użytkownikom usługi B2B w usłudze Azure AD Access w aplikacjach lokalnych](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Dowiedz się, jak [udzielić lokalnie zarządzanych kont partnerskich dostępu do zasobów w chmurze przy użyciu współpracy w usłudze Azure AD za pomocą usługi Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).