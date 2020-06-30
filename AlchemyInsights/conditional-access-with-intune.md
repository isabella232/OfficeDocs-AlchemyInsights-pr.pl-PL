---
title: Dostęp warunkowy z usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931446"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b067b-102">Dostęp warunkowy z usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="b067b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b067b-103">Korzystanie z **dostępu warunkowego** z usłudze Intune wymaga 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="b067b-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="b067b-104">Utwórz **zasady zgodności** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="b067b-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b067b-105">Na przykład urządzenie musi mieć pin co najmniej 6 cyfr, zanim zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="b067b-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="b067b-106">Utwórz **zasady dostępu warunkowego,** który określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="b067b-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="b067b-107">[Na przykład](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) urządzenie musi być zgodne przed dostępem do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="b067b-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="b067b-108">Upewnij się, że zarówno **zasady zgodności,** jak i **zasady dostępu warunkowego** są kierowane do pożądanych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="b067b-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="b067b-109">Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b067b-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="b067b-110">**Pomocne linki:**</span><span class="sxs-lookup"><span data-stu-id="b067b-110">**Helpful links:**</span></span>

[<span data-ttu-id="b067b-111">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="b067b-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="b067b-112">Rozwiązywanie problemów z urzędem certyfikacji</span><span class="sxs-lookup"><span data-stu-id="b067b-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b067b-113">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="b067b-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="b067b-114">Aby chronić pocztę e-mail (Exchange online) przed dostępem przez niezgodne urządzenia, oba dokumenty muszą być przestrzegane:</span><span class="sxs-lookup"><span data-stu-id="b067b-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="b067b-115">Ochrona dostępu do poczty e-mail przed urządzeniami za pomocą usługi EAS</span><span class="sxs-lookup"><span data-stu-id="b067b-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="b067b-116">Ochrona dostępu do poczty e-mail przed urządzeniami przy użyciu nowoczesnych klientów uwierzytelniania, takich jak Outlook</span><span class="sxs-lookup"><span data-stu-id="b067b-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)