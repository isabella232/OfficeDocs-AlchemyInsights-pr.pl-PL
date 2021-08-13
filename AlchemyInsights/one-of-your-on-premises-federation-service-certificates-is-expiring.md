---
title: Wygasa jeden z lokalnych certyfikatów usługi federejnej
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985227"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Wygasa jeden z lokalnych certyfikatów usługi federejnej

Aby rozwiązać ten problem, wykonaj następujące czynności:
  
- Zainstaluj Microsoft Azure Active Directory modułu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do Azure Active Directory [PowerShell dla Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Wykonaj czynności opisane w sekcji "Scenariusz 1: Certyfikat podpisywania tokenu usług AD FS wygasł" w sekcji "Wystąpił problem z dostępem do witryny" z usług AD FS, gdy użytkownik federowany loguje się do usługi [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)lub Intune.
    
- Postępuj zgodnie z instrukcjami w tece Jak aktualizować lub naprawiać ustawienia domeny federacji w usłudze [Microsoft 365, Azure lub Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Aby uzyskać więcej informacji na temat odnawiania certyfikatów federacji, zobacz Odnawianie certyfikatów [dla usług O365 i Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

