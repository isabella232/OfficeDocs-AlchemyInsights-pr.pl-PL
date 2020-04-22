---
title: Synchronizacja upn wyłączona
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726114"
---
# <a name="upn-sync-disabled"></a>Synchronizacja upn wyłączona

Jeśli synchronizacja z usługą Azure AD została rozpoczęta przed 30 marca 2016 r., uruchom następujące polecenie cmdlet usługi Azure AD PowerShell, aby włączyć miękkie dopasowanie sieci UPN tylko dla twojej organizacji:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Włącz $True**
  
Dopasowanie nietrowane w sieci UPN jest automatycznie włączane dla organizacji, które rozpoczęły synchronizację z usługą Azure AD w dniu lub później 30 marca 2016 r.
  
Aby dowiedzieć się więcej o włączaniu dopasowania programowego UPN i innych funkcji synchronizacji, zobacz [funkcje usługi synchronizacji usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

