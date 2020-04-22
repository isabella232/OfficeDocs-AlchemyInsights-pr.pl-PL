---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707921"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="3dd54-102">Rozwiązywanie problemów z dostarczaniem kodu błędu 550 5.4.1 Odmowa dostępu do przekaźnika</span><span class="sxs-lookup"><span data-stu-id="3dd54-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="3dd54-103">Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec odbijaniu podczas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) wchodzenia do sieci firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3dd54-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="3dd54-104">Spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="3dd54-104">Try the following:</span></span>

1. <span data-ttu-id="3dd54-105">Określ, czy problem dotyczy całej domeny, czy pojedynczego adresu e-mail:</span><span class="sxs-lookup"><span data-stu-id="3dd54-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="3dd54-106">Cała domena: czasami domena musi być zsynchronizowana; spróbuj [skonfigurować domenę na Wewnętrzną, a następnie wróć do Autorytatywny](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="3dd54-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="3dd54-107">Pojedynczy adres e-mail: czasami adres musi być zsynchronizowany; zmiana adresu proxy smtp, a następnie zmiana go z powrotem może pomóc.</span><span class="sxs-lookup"><span data-stu-id="3dd54-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="3dd54-108">Określ, czy problem jest specyficzny dla grupy lub folderu publicznego.</span><span class="sxs-lookup"><span data-stu-id="3dd54-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="3dd54-109">W przypadku niektórych typów obiektów obiekty mogą wymagać ręcznego utworzenia w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3dd54-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="3dd54-110">Jeśli potrzebujesz dodatkowej pomocy, otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do którego wysyłasz), abyśmy mogli ci lepiej pomóc.</span><span class="sxs-lookup"><span data-stu-id="3dd54-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>