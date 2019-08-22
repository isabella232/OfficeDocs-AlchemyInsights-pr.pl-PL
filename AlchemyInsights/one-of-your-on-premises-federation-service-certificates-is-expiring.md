---
title: Jednym z certyfikatami usługi federacyjnej lokalnego wygasa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543575"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jednym z certyfikatami usługi federacyjnej lokalnego wygasa

Aby rozwiązać ten problem, wykonaj następujące kroki:
  
- Zainstaluj Microsoft Azure Active Directory moduł dla środowiska Windows PowerShell na komputerze (jeśli jeszcze nie jest zainstalowany moduł). Aby to zrobić, przejdź do [Azure Active Directory PowerShell dla wykresu](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Postępuj zgodnie z instrukcjami "scenariusz 1: wygasł certyfikat podpisywania tokenu programu AD FS" sekcja [błąd "Wystąpił problem z dostępem do witryny" w programie AD FS podczas użytkownika federacyjnego zarejestruje się w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Postępuj zgodnie z instrukcjami t[jak zaktualizować lub naprawa ustawień federacyjnych domeny w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Aby uzyskać więcej informacji na temat odnawiania certyfikatów Federacji zobacz [Odnawianie certyfikatu dla O365 i Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

