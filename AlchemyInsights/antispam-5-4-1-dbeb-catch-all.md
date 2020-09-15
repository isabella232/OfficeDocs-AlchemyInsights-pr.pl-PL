---
title: AntiSpam 5.4.1 DBEB-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717371"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="6aebb-102">Rozwiązywanie problemów dotyczących dostarczania kodu błędu 550 5.4.1 Przekazywanie dostępu</span><span class="sxs-lookup"><span data-stu-id="6aebb-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="6aebb-103">Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wchodzenia do sieci Microsoft Network.</span><span class="sxs-lookup"><span data-stu-id="6aebb-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="6aebb-104">Spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="6aebb-104">Try the following:</span></span>

1. <span data-ttu-id="6aebb-105">Ustal, czy problem dotyczy całej domeny, czy jednego adresu e-mail:</span><span class="sxs-lookup"><span data-stu-id="6aebb-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="6aebb-106">Cała domena: Czasami trzeba zsynchronizować domenę; Spróbuj [skonfigurować domenę jako wewnętrzną, a następnie ponownie na autorytatywną](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="6aebb-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="6aebb-107">Jeden adres e-mail: Czasami należy zsynchronizować adres; Zmiana adresu serwera proxy SMTP, a następnie jego ponownej zmiany może pomóc.</span><span class="sxs-lookup"><span data-stu-id="6aebb-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="6aebb-108">Ustal, czy problem dotyczy grupy, czy folderu publicznego.</span><span class="sxs-lookup"><span data-stu-id="6aebb-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="6aebb-109">W przypadku niektórych typów obiektów w usłudze Azure Active Directory może być konieczne ręczne utworzenie obiektu.</span><span class="sxs-lookup"><span data-stu-id="6aebb-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="6aebb-110">Jeśli potrzebujesz dodatkowej pomocy, Otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, na który wysyłasz), dzięki czemu możemy pomóc Ci lepiej.</span><span class="sxs-lookup"><span data-stu-id="6aebb-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>