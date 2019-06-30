---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388255"
---
<span data-ttu-id="1567a-103">Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.</span><span class="sxs-lookup"><span data-stu-id="1567a-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1567a-104">**Klucz rejestru**</span><span class="sxs-lookup"><span data-stu-id="1567a-104">**Registry key**</span></span>|<span data-ttu-id="1567a-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="1567a-105">**Type**</span></span>|<span data-ttu-id="1567a-106">**Wartość**</span><span class="sxs-lookup"><span data-stu-id="1567a-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1567a-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1567a-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1567a-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="1567a-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1567a-109">1</span><span class="sxs-lookup"><span data-stu-id="1567a-109">1</span></span>  <br/> |

<span data-ttu-id="1567a-110">Aby uzyskać więcej informacji zobacz [Włączanie uwierzytelniania nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="1567a-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1567a-111">ADAL jest włączona domyślnie w Office 365 ProPlus i 2016 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="1567a-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="1567a-112">> usług pulpitu zdalnego (RDS) wcześniej nosił nazwę usług terminalowych.</span><span class="sxs-lookup"><span data-stu-id="1567a-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  