---
title: Trwa wygasanie jednego z certyfikatów usług federacyjnych lokalnie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673507"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Trwa wygasanie jednego z certyfikatów usług federacyjnych lokalnie

Aby rozwiązać ten problem, wykonaj następujące czynności:
  
- Zainstaluj moduł Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (Jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do [programu Azure Active Directory PowerShell dla wykresu ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Postępuj zgodnie z instrukcjami podanymi w sekcji "scenariusz 1: certyfikat podpisywania tokenu usług AD FS wygasł" [w usłudze AD FS — błąd "Wystąpił problem z dostępem do witryny", gdy użytkownik federacyjny loguje się do usługi Microsoft 365, Azure lub Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Postępuj zgodnie z instrukcjami w temacie [Aktualizowanie lub naprawianie ustawień domeny federacyjnej w programie Microsoft 365, Azure lub Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Aby uzyskać więcej informacji na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów w usłudze Office 365 i usłudze Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

