---
title: AntiSpam 5.4.1 DbEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821457"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="eb27f-102">Rozwiązywanie problemów dotyczących dostarczania związanych z kodem błędu 550 5.4.1 Odmowa dostępu przekazywania</span><span class="sxs-lookup"><span data-stu-id="eb27f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="eb27f-103">Ten problem występuje podczas sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec zwrotom [zwrotnych](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wprowadzania sieci firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="eb27f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="eb27f-104">Wypróbuj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="eb27f-104">Try the following:</span></span>

1. <span data-ttu-id="eb27f-105">Określ, czy problem dotyczy całej domeny, czy pojedynczego adresu e-mail:</span><span class="sxs-lookup"><span data-stu-id="eb27f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="eb27f-106">Cała domena: czasami trzeba zsynchronizować domenę. Spróbuj [zmienić domenę na Wewnętrzna, a następnie z powrotem na Autorytatywny.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="eb27f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="eb27f-107">Jeden adres e-mail: Czasami trzeba zsynchronizować adres; Zmiana adresu serwera proxy SMTP, a następnie jego zmiana z powrotem może pomóc.</span><span class="sxs-lookup"><span data-stu-id="eb27f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="eb27f-108">Określanie, czy problem jest specyficzny dla grupy, czy folderu publicznego.</span><span class="sxs-lookup"><span data-stu-id="eb27f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="eb27f-109">W przypadku niektórych typów obiektów może być konieczne ich ręczne utworzenie w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eb27f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="eb27f-110">Jeśli potrzebujesz dodatkowej pomocy, otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do który wysyłasz), abyśmy pomogli Ci pomóc.</span><span class="sxs-lookup"><span data-stu-id="eb27f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>