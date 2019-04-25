---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402749"
---
<span data-ttu-id="a9de0-103">Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.</span><span class="sxs-lookup"><span data-stu-id="a9de0-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="a9de0-104">**Klucz rejestru**</span><span class="sxs-lookup"><span data-stu-id="a9de0-104">**Registry key**</span></span>|<span data-ttu-id="a9de0-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="a9de0-105">**Type**</span></span>|<span data-ttu-id="a9de0-106">**Wartość**</span><span class="sxs-lookup"><span data-stu-id="a9de0-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a9de0-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="a9de0-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="a9de0-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="a9de0-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="a9de0-109">1</span><span class="sxs-lookup"><span data-stu-id="a9de0-109">1</span></span>  <br/> |
   
<span data-ttu-id="a9de0-110">Aby uzyskać więcej informacji zobacz [Włączanie uwierzytelniania nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a9de0-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="a9de0-111">ADAL jest włączona domyślnie w Office 365 ProPlus i 2016 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="a9de0-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="a9de0-112">> usług pulpitu zdalnego (RDS) wcześniej nosił nazwę usług terminalowych.</span><span class="sxs-lookup"><span data-stu-id="a9de0-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

