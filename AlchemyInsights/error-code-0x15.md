---
title: Kod błędu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jeśli podczas włączania wdrożeń usługi RDS (Remote Desktop Services) pojawia się błąd, należy rozważyć włączenie usługi ADAL przez edycję rejestru.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703148"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="fcd86-103">Błąd podczas aktywacji pakietu Office 2013 w usługach pulpitu zdalnego</span><span class="sxs-lookup"><span data-stu-id="fcd86-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="fcd86-104">Jeśli podczas włączania wdrożeń usługi RDS (Remote Desktop Services) pojawia się błąd, należy rozważyć włączenie usługi ADAL przez edycję rejestru.</span><span class="sxs-lookup"><span data-stu-id="fcd86-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="fcd86-105">**Klucz rejestru**</span><span class="sxs-lookup"><span data-stu-id="fcd86-105">**Registry key**</span></span>|<span data-ttu-id="fcd86-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="fcd86-106">**Type**</span></span>|<span data-ttu-id="fcd86-107">**Wartość**</span><span class="sxs-lookup"><span data-stu-id="fcd86-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fcd86-108">HKEY_CURRENT_USER\Oprogramowanie\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="fcd86-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="fcd86-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="fcd86-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="fcd86-110">1</span><span class="sxs-lookup"><span data-stu-id="fcd86-110">1</span></span>  <br/> |

<span data-ttu-id="fcd86-111">Aby uzyskać więcej informacji, zobacz [Włączanie nowoczesnego uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="fcd86-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="fcd86-112">Usługa ADAL jest domyślnie włączona w usłudze Microsoft 365 Apps dla przedsiębiorstw i pakiecie Office 2016.</span><span class="sxs-lookup"><span data-stu-id="fcd86-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="fcd86-113">Usługi pulpitu zdalnego (RDS) były wcześniej nazywane usługami terminalowymi.</span><span class="sxs-lookup"><span data-stu-id="fcd86-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  