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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527037"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="56a85-103">Wystąpił błąd podczas aktywacji pakietu Office 2013 na usług pulpitu zdalnego</span><span class="sxs-lookup"><span data-stu-id="56a85-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="56a85-104">Jeśli otrzymujesz komunikat o błędzie podczas aktywowania pakietu Office 2013 we wdrożeniach usług pulpitu zdalnego (RDS), należy rozważyć włączenie ADAL przez edycję rejestru.</span><span class="sxs-lookup"><span data-stu-id="56a85-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="56a85-105">**Klucz rejestru**</span><span class="sxs-lookup"><span data-stu-id="56a85-105">**Registry key**</span></span>|<span data-ttu-id="56a85-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="56a85-106">**Type**</span></span>|<span data-ttu-id="56a85-107">**Wartość**</span><span class="sxs-lookup"><span data-stu-id="56a85-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="56a85-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="56a85-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="56a85-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="56a85-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="56a85-110">1</span><span class="sxs-lookup"><span data-stu-id="56a85-110">1</span></span>  <br/> |

<span data-ttu-id="56a85-111">Aby uzyskać więcej informacji zobacz [Włączanie uwierzytelniania nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="56a85-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="56a85-112">ADAL jest włączona domyślnie w Office 365 ProPlus i 2016 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="56a85-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="56a85-113">Usługi pulpitu zdalnego (RDS) wcześniej nosił nazwę usług terminalowych.</span><span class="sxs-lookup"><span data-stu-id="56a85-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  