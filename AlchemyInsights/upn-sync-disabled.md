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
# <a name="upn-sync-disabled"></a><span data-ttu-id="e1c2a-102">Synchronizacja UPN wyłączona</span><span class="sxs-lookup"><span data-stu-id="e1c2a-102">UPN sync disabled</span></span>

<span data-ttu-id="e1c2a-103">Jeśli rozpoczęto synchronizację z Azure AD przed 30 marca 2016, uruchom następujące polecenia środowiska AD PowerShell Azure umożliwiające dopasowanie miękkie UPN dla organizacji tylko:</span><span class="sxs-lookup"><span data-stu-id="e1c2a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="e1c2a-104">**Zestaw MsolDirSyncFeature-funkcja EnableSoftMatchOnUpn-Włącz $True**</span><span class="sxs-lookup"><span data-stu-id="e1c2a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="e1c2a-105">UPN miękkim dopasowaniem jest automatycznie włączona dla organizacji, które rozpoczęły synchronizacji do Azure AD lub po 30 marca 2016.</span><span class="sxs-lookup"><span data-stu-id="e1c2a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="e1c2a-106">Aby dowiedzieć się więcej o włączaniu miękkie dopasowania na główną nazwę użytkownika i inne funkcje synchronizacji, zobacz [funkcje usługi synchronizacji Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="e1c2a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

