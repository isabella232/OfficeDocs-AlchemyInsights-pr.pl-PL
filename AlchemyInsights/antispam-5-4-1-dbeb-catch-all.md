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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964257"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="b06ac-102">Rozwiązywanie problemów z dostarczaniem kodu błędu 550 5.4.1 odmowa dostępu do przekaźnika</span><span class="sxs-lookup"><span data-stu-id="b06ac-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="b06ac-103">Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wprowadzania sieci 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="b06ac-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="b06ac-104">Wypróbuj następujące:</span><span class="sxs-lookup"><span data-stu-id="b06ac-104">Try the following:</span></span>

1. <span data-ttu-id="b06ac-105">Określ, czy problem dotyczy całej domeny, czy jednego adresu e-mail:</span><span class="sxs-lookup"><span data-stu-id="b06ac-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="b06ac-106">Cała domena: czasami domena musi być synchronizowana; Spróbuj [ustawić domenę jako wewnętrzną, a następnie wróć do autorytatywnych](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="b06ac-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="b06ac-107">Pojedynczy adres e-mail: Czasami adres musi być zsynchronizowany; zmienić adres serwera proxy SMTP, a następnie zmienić go z powrotem może pomóc.</span><span class="sxs-lookup"><span data-stu-id="b06ac-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="b06ac-108">Określić, czy problem jest specyficzny dla grupy lub folderu publicznego.</span><span class="sxs-lookup"><span data-stu-id="b06ac-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="b06ac-109">W przypadku niektórych typów obiektów może być konieczne ręczne utworzenie w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b06ac-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="b06ac-110">Jeśli potrzebujesz dodatkowej pomocy, Otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do którego wysyłasz), abyśmy mogli pomóc Ci lepiej.</span><span class="sxs-lookup"><span data-stu-id="b06ac-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>