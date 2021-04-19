---
title: Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813482"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="4c3f5-102">Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego</span><span class="sxs-lookup"><span data-stu-id="4c3f5-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="4c3f5-103">Aby uzyskać najnowsze informacje na temat sposobu łączenia się z programem PowerShell dla usługi Exchange Online bez używania uwierzytelniania podstawowego, [przejdź tutaj](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="4c3f5-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="4c3f5-104">Moduł V2 programu PowerShell nie używa uwierzytelniania podstawowego.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="4c3f5-105">Pamiętaj, że na Twoim komputerze klienckim wciąż musi być włączone uwierzytelnianie podstawowe.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="4c3f5-106">Nowy moduł programu PowerShell V2 korzysta z nowoczesnego uwierzytelniania do nawiązywania połączeń w celu włączenia wszystkich poleceń cmdlet V2 opartych na usłudze REST.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="4c3f5-107">Poza poleceniami cmdlet V2 pozwala on również uzyskać dostęp do starszych poleceń cmdlet RPS (Remote PowerShell — zdalna obsługa programu PowerShell), co wymaga ustanowienia sesji zdalnej programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="4c3f5-108">Ustanowienie sesji RPS na komputerze z systemem Windows wymaga, aby na komputerze klienckim było włączone uwierzytelnianie podstawowe, mimo że w celu uwierzytelnienia usługi moduł wykorzystuje nowoczesne uwierzytelnianie.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="4c3f5-109">Potok uwierzytelniania podstawowego WinRM jest wykorzystywany do transportu tokenów nowoczesnego uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="4c3f5-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="4c3f5-110">Jeśli na komputerze klienckim wyłączone jest uwierzytelnianie podstawowe WinRM, nowe polecenia cmdlet V2 będą nadal działać (ale nie będą działać starsze polecenia cmdlet RPS).</span><span class="sxs-lookup"><span data-stu-id="4c3f5-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
