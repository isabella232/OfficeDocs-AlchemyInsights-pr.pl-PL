---
title: Synchronizacja głównej nazwy użytkownika jest wyłączona
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749524"
---
# <a name="upn-sync-disabled"></a>Synchronizacja głównej nazwy użytkownika jest wyłączona

Jeśli synchronizacja z usługą Azure AD została rozpoczęta przed 30 marca 2016, uruchom polecenie cmdlet programu PowerShell usługi Azure AD, aby włączyć opcję wstępnego dopasowania głównej nazwy użytkownika tylko dla swojej organizacji:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
Funkcja automatycznego dopasowania głównej nazwy użytkownika jest automatycznie włączana dla organizacji, które rozpoczęły synchronizację z usługą Azure AD w dniu lub po 30 marca 2016.
  
Aby dowiedzieć się więcej o włączaniu łagodnych odpowiedników dla głównej nazwy użytkownika i innych funkcji synchronizacji, zobacz [funkcje usługi Microsoft Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

