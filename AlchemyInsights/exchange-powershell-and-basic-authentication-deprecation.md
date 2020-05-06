---
title: Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015699"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="bccaa-102">Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego</span><span class="sxs-lookup"><span data-stu-id="bccaa-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="bccaa-103">Aby uzyskać najnowsze informacje na temat sposobu łączenia się z programem PowerShell dla usługi Exchange Online bez używania uwierzytelniania podstawowego, [przejdź tutaj](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="bccaa-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="bccaa-104">Pamiętaj, że na Twoim komputerze klienckim wciąż musi być włączone uwierzytelnianie podstawowe.</span><span class="sxs-lookup"><span data-stu-id="bccaa-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="bccaa-105">Nowy moduł programu PowerShell V2 korzysta z nowoczesnego uwierzytelniania do nawiązywania połączeń w celu włączenia wszystkich poleceń cmdlet V2 opartych na usłudze REST.</span><span class="sxs-lookup"><span data-stu-id="bccaa-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="bccaa-106">Poza poleceniami cmdlet V2 pozwala on również uzyskać dostęp do starszych poleceń cmdlet RPS (Remote PowerShell — zdalna obsługa programu PowerShell), co wymaga ustanowienia sesji zdalnej programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bccaa-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="bccaa-107">Ustanowienie sesji RPS na komputerze z systemem Windows wymaga, aby na komputerze klienckim było włączone uwierzytelnianie podstawowe, mimo że w celu uwierzytelnienia usługi moduł wykorzystuje nowoczesne uwierzytelnianie.</span><span class="sxs-lookup"><span data-stu-id="bccaa-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="bccaa-108">Potok uwierzytelniania podstawowego WinRM jest wykorzystywany do transportu tokenów nowoczesnego uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="bccaa-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="bccaa-109">Jeśli na komputerze klienckim wyłączone jest uwierzytelnianie podstawowe WinRM, nowe polecenia cmdlet V2 będą nadal działać (ale nie będą działać starsze polecenia cmdlet RPS).</span><span class="sxs-lookup"><span data-stu-id="bccaa-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
