---
title: Synchronizacja UPN wyłączona
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423568"
---
# <a name="upn-sync-disabled"></a>Synchronizacja UPN wyłączona

Jeśli rozpoczęto synchronizację z Azure AD przed 30 marca 2016, uruchom następujące polecenia środowiska AD PowerShell Azure umożliwiające dopasowanie miękkie UPN dla organizacji tylko:
  
 **Zestaw MsolDirSyncFeature-funkcja EnableSoftMatchOnUpn-Włącz $True**
  
UPN miękkim dopasowaniem jest automatycznie włączona dla organizacji, które rozpoczęły synchronizacji do Azure AD lub po 30 marca 2016.
  
Aby dowiedzieć się więcej o włączaniu miękkie dopasowania na główną nazwę użytkownika i inne funkcje synchronizacji, zobacz [funkcje usługi synchronizacji Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

