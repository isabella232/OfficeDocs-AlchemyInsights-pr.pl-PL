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
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482912"
---
# <a name="upn-sync-disabled"></a>Synchronizacja UPN wyłączona

Jeśli rozpoczęto synchronizację z Azure AD przed 30 marca 2016, uruchom następujące polecenia środowiska AD PowerShell Azure umożliwiające dopasowanie miękkie UPN dla organizacji tylko:
  
 **Zestaw MsolDirSyncFeature-funkcja EnableSoftMatchOnUpn-Włącz $True**
  
UPN miękkim dopasowaniem jest automatycznie włączona dla organizacji, które rozpoczęły synchronizacji do Azure AD lub po 30 marca 2016.
  
Aby dowiedzieć się więcej o włączaniu miękkie dopasowania na główną nazwę użytkownika i inne funkcje synchronizacji, zobacz [funkcje usługi synchronizacji Azure Połącz AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

