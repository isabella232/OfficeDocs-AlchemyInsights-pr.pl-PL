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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782161"
---
# <a name="upn-sync-disabled"></a>Wyłączona synchronizacja upn

Jeśli rozpoczęto synchronizację z usługą Azure AD przed 30 marca 2016 r., uruchom następujące polecenie cmdlet programu PowerShell usługi Azure AD, aby włączyć "miękkie dopasowanie" upn tylko dla Twojej organizacji:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Programowe dopasowanie upn jest automatycznie włączone dla organizacji, które rozpoczęła synchronizację z usługą Azure AD w dniu 30 marca 2016 r. lub później.
  
Aby dowiedzieć się więcej o włączaniu funkcji "miękkiego dopasowania" w upn i innych funkcjach synchronizacji, zobacz Funkcje usługi [synchronizacji Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

