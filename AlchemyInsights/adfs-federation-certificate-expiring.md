---
title: Wygasanie certyfikatu Federacji usług ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686757"
---
# <a name="adfs-federation-certificate-expiring"></a>Wygasanie certyfikatu Federacji usług ADFS

Aby rozwiązać ten problem, wykonaj następujące czynności:
  
1. Zainstaluj moduł Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (Jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do obszaru [Zarządzanie usługą Azure AD przy użyciu programu Windows PowerShell](https://aka.ms/aadposh).

2. Postępuj zgodnie z instrukcjami podanymi w sekcji "scenariusz 1: certyfikat podpisywania tokenu usług AD FS wygasł" [w usłudze AD FS — błąd "Wystąpił problem z dostępem do witryny", gdy użytkownik federacyjny loguje się do usługi Microsoft 365, Azure lub Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Postępuj zgodnie z instrukcjami w artykule [Aktualizowanie lub naprawianie ustawień domeny federacyjnej w usłudze Microsoft, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Aby dowiedzieć się więcej na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów federacyjnych dla systemu Microsoft 365 i usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
