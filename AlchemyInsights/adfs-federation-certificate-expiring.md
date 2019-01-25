---
title: ADFS federacyjnej Wygasający certyfikat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483086"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS federacyjnej Wygasający certyfikat

Aby rozwiązać ten problem, wykonaj następujące kroki:
  
1. Zainstaluj Microsoft Azure Active Directory moduł dla środowiska Windows PowerShell na komputerze (jeśli jeszcze nie jest zainstalowany moduł). Aby to zrobić, przejdź do [Zarządzaj Azure AD przy użyciu środowiska Windows PowerShell](https://aka.ms/aadposh).
    
2. Postępuj zgodnie z instrukcjami "scenariusz 1: wygasł certyfikat podpisywania tokenu programu AD FS" sekcja [błąd "Wystąpił problem z dostępem do witryny" w programie AD FS podczas użytkownika federacyjnego zarejestruje się w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Postępuj zgodnie z instrukcjami [jak zaktualizować lub naprawa ustawień federacyjnych domeny w usłudze Office 365, Azure lub Windows Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Aby dowiedzieć się więcej na temat odnawiania certyfikatów federacyjnej, zobacz [Odnawianie certyfikatów Federacji dla usługi Office 365 i Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

