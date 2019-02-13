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
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921718"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="81a15-102">Synchronizacja UPN wyłączona</span><span class="sxs-lookup"><span data-stu-id="81a15-102">UPN sync disabled</span></span>

<span data-ttu-id="81a15-103">Jeśli rozpoczęto synchronizację z Azure AD przed 30 marca 2016, uruchom następujące polecenia środowiska AD PowerShell Azure umożliwiające dopasowanie miękkie UPN dla organizacji tylko:</span><span class="sxs-lookup"><span data-stu-id="81a15-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="81a15-104">**Zestaw MsolDirSyncFeature-funkcja EnableSoftMatchOnUpn-Włącz $True**</span><span class="sxs-lookup"><span data-stu-id="81a15-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="81a15-105">UPN miękkim dopasowaniem jest automatycznie włączona dla organizacji, które rozpoczęły synchronizacji do Azure AD lub po 30 marca 2016.</span><span class="sxs-lookup"><span data-stu-id="81a15-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="81a15-106">Aby dowiedzieć się więcej o włączaniu miękkie dopasowania na główną nazwę użytkownika i inne funkcje synchronizacji, zobacz [funkcje usługi synchronizacji Azure Połącz AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="81a15-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

