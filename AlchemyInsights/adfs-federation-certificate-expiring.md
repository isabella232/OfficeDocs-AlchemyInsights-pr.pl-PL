---
title: Wygasający certyfikat federacji usług ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821961"
---
# <a name="adfs-federation-certificate-expiring"></a>Wygasający certyfikat federacji usług ADFS

Aby rozwiązać ten problem, wykonaj następujące czynności:
  
1. Zainstaluj moduł usługi Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do tematu [Zarządzanie usługą Azure AD przy użyciu programu Windows PowerShell.](https://aka.ms/aadposh)

2. Wykonaj czynności opisane w sekcji "Scenariusz 1: Certyfikat podpisywania tokenu usług AD FS wygasł" w sekcji "Wystąpił problem z dostępem do witryny" z usług AD FS, gdy użytkownik federowany loguje się do platformy [Microsoft 365,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)platformy Azure lub Intune.

3. Wykonaj czynności opisane w tece Aktualizowanie lub naprawianie ustawień [domeny federacji na platformie Microsoft, Azure lub Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Aby dowiedzieć się więcej o odnawianiu certyfikatów federacji, zobacz Odnawianie certyfikatów federacji dla platformy [Microsoft 365 i usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
