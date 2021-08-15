---
title: Wyłączona synchronizacja upn
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038122"
---
# <a name="upn-sync-disabled"></a>Wyłączona synchronizacja upn

Jeśli rozpoczęto synchronizację z usługą Azure AD przed 30 marca 2016 r., uruchom następujące polecenie cmdlet programu PowerShell usługi Azure AD, aby włączyć "miękkie dopasowanie" upn tylko dla Twojej organizacji:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Programowe dopasowanie upn jest automatycznie włączone dla organizacji, które rozpoczęła synchronizację z usługą Azure AD w dniu 30 marca 2016 r. lub później.
  
Aby dowiedzieć się więcej o włączaniu funkcji "miękkiego dopasowania" w upn i innych funkcjach synchronizacji, zobacz Funkcje usługi synchronizacji Połączenie [Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

