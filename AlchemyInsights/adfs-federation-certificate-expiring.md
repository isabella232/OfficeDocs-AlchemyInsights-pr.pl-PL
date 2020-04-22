---
title: Wygasa certyfikat federacyjny usługi ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710417"
---
# <a name="adfs-federation-certificate-expiring"></a>Wygasa certyfikat federacyjny usługi ADFS

Aby rozwiązać ten problem, wykonaj następujące kroki:
  
1. Zainstaluj moduł usługi Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do [zarządzania usługą Azure AD przy użyciu programu Windows PowerShell](https://aka.ms/aadposh).

2. Wykonaj kroki opisane w sekcji "Scenariusz 1: Wygasł certyfikat podpisywania tokenów usług AD FS" w sekcji ["Wystąpił problem z dostępem do witryny" z usług AD FS, gdy federowany użytkownik loguje się do usługi Microsoft 365, platformy Azure lub usługi Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Wykonaj kroki opisane w [sekcji Aktualizowanie lub naprawianie ustawień domeny federacyjnej w firmie Microsoft, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Aby dowiedzieć się więcej o odnawianiu certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów federacyjnych dla usługi Microsoft 365 i usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
