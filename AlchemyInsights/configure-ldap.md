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
# <a name="configure-ldap"></a><span data-ttu-id="ac884-102">Konfigurowanie protokołu LDAP</span><span class="sxs-lookup"><span data-stu-id="ac884-102">Configure LDAP</span></span>

<span data-ttu-id="ac884-103">Aby skonfigurować protokół LDAP, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ac884-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="ac884-104">Sprawdź kondycję Twojej domeny w witrynie [Azure Portal](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="ac884-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="ac884-105">Upewnij się, że jest dostępny prawidłowy abonament Azure AD, a usługi domenowe usługi Azure AD zostały włączone.</span><span class="sxs-lookup"><span data-stu-id="ac884-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="ac884-106">Certyfikat wymagany do włączenia bezpiecznego protokołu LDAP musi być uzyskiwany z zaufanego publicznego urzędu certyfikacji lub jako certyfikat z podpisem własnym.</span><span class="sxs-lookup"><span data-stu-id="ac884-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="ac884-107">Upewnij się, że certyfikat jest zgodny z wymaganymi [wskazówkami](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="ac884-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="ac884-108">**Nieprawidłowy certyfikat**</span><span class="sxs-lookup"><span data-stu-id="ac884-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="ac884-109">Aby odnowić certyfikat, postępuj zgodnie z instrukcjami, aby utworzyć nowy certyfikat i przekazać go [ponownie: Konfigurowanie protokołu LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ac884-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="ac884-110">Aby rozwiązać znany problem z zabezpieczeniami alertów LDAP w usługach domenowych Active Directory Azure, zobacz temat [rozpoznawanie alertów LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ac884-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
