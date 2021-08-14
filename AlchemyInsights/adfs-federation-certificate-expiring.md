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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952979"
---
# <a name="adfs-federation-certificate-expiring"></a>Wygasający certyfikat federacji usług ADFS

Aby rozwiązać ten problem, wykonaj następujące czynności:
  
1. Zainstaluj Microsoft Azure Active Directory modułu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany). Aby to zrobić, przejdź do [tematu Zarządzanie usługą Azure AD przy użyciu Windows PowerShell.](https://aka.ms/aadposh)

2. Wykonaj czynności opisane w sekcji "Scenariusz 1: Certyfikat podpisywania tokenu usług AD FS wygasł" w sekcji "Wystąpił problem z dostępem do witryny" z usług AD FS, gdy użytkownik federowany loguje się do usługi [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)lub Intune.

3. Wykonaj czynności opisane w tece Aktualizowanie lub naprawianie ustawień [domeny federacji na platformie Microsoft, Azure lub Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Aby dowiedzieć się więcej o odnawianiu certyfikatów federacji, zobacz Odnawianie certyfikatów federacji dla Microsoft 365 [i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
