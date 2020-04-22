---
title: Wygasa jeden z lokalnych certyfikatów usługi federacyjnej
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761393"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Wygasa jeden z lokalnych certyfikatów usługi federacyjnej

Aby rozwiązać ten problem, wykonaj następujące kroki:
  
- Zainstaluj moduł usługi Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do [programu Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Wykonaj kroki opisane w sekcji "Scenariusz 1: Wygasł certyfikat podpisywania tokenów usług AD FS" w sekcji ["Wystąpił problem z dostępem do witryny" z usług AD FS, gdy federowany użytkownik loguje się do usługi Office 365, platformy Azure lub usługi Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Wykonaj kroki opisane w obszarze jak[zaktualizować lub naprawić ustawienia domeny federacyjnej w usłudze Office 365, platformie Azure lub usłudze Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Aby uzyskać więcej informacji na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów dla usług O365 i Usługi Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

