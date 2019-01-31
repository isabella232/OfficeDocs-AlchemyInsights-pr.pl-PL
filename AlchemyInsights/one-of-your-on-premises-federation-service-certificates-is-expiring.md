---
title: Jednym z certyfikatami usługi federacyjnej lokalnego wygasa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 9e2e1a1dd2993b2a02b4405db8a707b23ff4af16
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658917"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jednym z certyfikatami usługi federacyjnej lokalnego wygasa

Aby rozwiązać ten problem, wykonaj następujące kroki:
  
- Zainstaluj Microsoft Azure Active Directory moduł dla środowiska Windows PowerShell na komputerze (jeśli jeszcze nie jest zainstalowany moduł). Aby to zrobić, przejdź do [Azure Active Directory PowerShell dla wykresu](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Postępuj zgodnie z instrukcjami "scenariusz 1: wygasł certyfikat podpisywania tokenu programu AD FS" sekcja [błąd "Wystąpił problem z dostępem do witryny" w programie AD FS podczas użytkownika federacyjnego zarejestruje się w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Postępuj zgodnie z instrukcjami t[jak zaktualizować lub naprawa ustawień federacyjnych domeny w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Aby uzyskać więcej informacji na temat odnawiania certyfikatów Federacji zobacz [Odnawianie certyfikatu dla O365 i Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

