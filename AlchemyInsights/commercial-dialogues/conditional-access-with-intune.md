---
title: Korzystanie z dostępu warunkowego w usłudze Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749258"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="6d2f5-102">Korzystanie z dostępu warunkowego w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="6d2f5-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="6d2f5-103">Korzystanie z dostępu warunkowego w usłudze Intune wymaga 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="6d2f5-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="6d2f5-104">Utwórz zasady zgodności, aby zdefiniować ustawienia, które muszą być spełnione, aby urządzenie zostało uznane za zgodne. Na przykład urządzenie musi mieć co najmniej 6-cyfrowy numer PIN, aby zostało uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="6d2f5-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="6d2f5-105">Utwórz zasady dostępu warunkowego definiujące zasoby, które są chronione oraz wymagania, które należy spełnić, aby uzyskać do nich dostęp. Na przykład urządzenie musi być zgodne, aby uzyskać dostęp do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="6d2f5-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="6d2f5-106">Upewnij się, że zarówno zasady zgodności, jak i zasady dostępu warunkowego są kierowane do odpowiednich grup użytkowników. Może to wymagać utworzenia konkretnych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6d2f5-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="6d2f5-107">Przeczytaj więcej...</span><span class="sxs-lookup"><span data-stu-id="6d2f5-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
