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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885573"
---
# <a name="configure-ldap"></a>Konfigurowanie protokołu LDAP

Aby skonfigurować protokół LDAP, wykonaj następujące czynności:

1. Sprawdź kondycję Twojej domeny w witrynie [Azure Portal](https://aka.ms/aadds-health).
1. Upewnij się, że jest dostępny prawidłowy abonament Azure AD, a usługi domenowe usługi Azure AD zostały włączone.
1. Certyfikat wymagany do włączenia bezpiecznego protokołu LDAP musi być uzyskiwany z zaufanego publicznego urzędu certyfikacji lub jako certyfikat z podpisem własnym.
1. Upewnij się, że certyfikat jest zgodny z wymaganymi [wskazówkami](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Nieprawidłowy certyfikat**
1. Aby odnowić certyfikat, postępuj zgodnie z instrukcjami, aby utworzyć nowy certyfikat i przekazać go [ponownie: Konfigurowanie protokołu LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Aby rozwiązać znany problem z zabezpieczeniami alertów LDAP w usługach domenowych Active Directory Azure, zobacz temat [rozpoznawanie alertów LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
