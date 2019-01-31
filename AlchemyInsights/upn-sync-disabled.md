---
title: Synchronizacja UPN wyłączona
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657981"
---
# <a name="upn-sync-disabled"></a>Synchronizacja UPN wyłączona

Jeśli rozpoczęto synchronizację z Azure AD przed 30 marca 2016, uruchom następujące polecenia środowiska AD PowerShell Azure umożliwiające dopasowanie miękkie UPN dla organizacji tylko:
  
 **Zestaw MsolDirSyncFeature-funkcja EnableSoftMatchOnUpn-Włącz $True**
  
UPN miękkim dopasowaniem jest automatycznie włączona dla organizacji, które rozpoczęły synchronizacji do Azure AD lub po 30 marca 2016.
  
Aby dowiedzieć się więcej o włączaniu miękkie dopasowania na główną nazwę użytkownika i inne funkcje synchronizacji, zobacz [funkcje usługi synchronizacji Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

