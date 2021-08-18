---
title: Konfigurowanie protokołu LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090422"
---
# <a name="configure-ldap"></a>Konfigurowanie protokołu LDAP

Aby skonfigurować LDAP, wykonaj następujące czynności:

1. Sprawdź kondycję domeny w portalu [Azure Portal.](https://aka.ms/aadds-health)
1. Upewnij się, że jest dostępna ważna subskrypcja usługi Azure AD i że włączono usługi domenowe Azure AD.
1. Certyfikat wymagany do włączenia bezpiecznego protokołu LDAP musi być uzyskany od zaufanego publicznego urzędu certyfikacji lub certyfikatem z podpisem własnym.
1. Upewnij się, że certyfikat jest zgodny z [wymaganymi wytycznymi.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Nieprawidłowy certyfikat**
1. Aby odnowić certyfikat, postępuj zgodnie z instrukcjami w celu utworzenia nowego certyfikatu i ponownego załadowania: [Konfigurowanie LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Aby rozwiązać znany problem z alertami LDAP w usługach domenowych Azure Active Directory, zobacz [Rozwiązywanie alertów LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
