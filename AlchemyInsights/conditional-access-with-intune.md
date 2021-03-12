---
title: Dostęp warunkowy w usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704796"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c8b8a-102">Dostęp warunkowy w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="c8b8a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c8b8a-103">Korzystanie  **z dostępu warunkowego**  w usłudze Intune wymaga 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="c8b8a-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="c8b8a-104">Utwórz zasady  **zgodności** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows),](https://docs.microsoft.com//intune/compliance-policy-create-windows)aby zdefiniować ustawienia, które muszą być spełnione, aby urządzenie zostało uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c8b8a-105">Na przykład urządzenie musi mieć co najmniej 6-cyfrowy numer PIN, aby zostało uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="c8b8a-106">Utwórz zasady **dostępu warunkowego**  definiujące zasoby, które są chronione, oraz warunki, które muszą zostać spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="c8b8a-107">[Na przykład urządzenie musi](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  być zgodne, aby uzyskać dostęp do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="c8b8a-108">Upewnij  **się, że zarówno zasady zgodności,** jak i zasady dostępu warunkowego są kierowane do odpowiednich grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="c8b8a-109">Może to wymagać utworzenia konkretnych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8b8a-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="c8b8a-110">**Przydatne linki:**</span><span class="sxs-lookup"><span data-stu-id="c8b8a-110">**Helpful links:**</span></span>

[<span data-ttu-id="c8b8a-111">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="c8b8a-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c8b8a-112">Rozwiązywanie problemów z urzędu certyfikacji</span><span class="sxs-lookup"><span data-stu-id="c8b8a-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c8b8a-113">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="c8b8a-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="c8b8a-114">Aby chronić pocztę e-mail (usługę Exchange Online) przed dostępem przez urządzenia nieuprawniane, należy przestrzegać obu dokumentów:</span><span class="sxs-lookup"><span data-stu-id="c8b8a-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="c8b8a-115">Ochrona dostępu do poczty e-mail przed urządzeniami za pomocą eas</span><span class="sxs-lookup"><span data-stu-id="c8b8a-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="c8b8a-116">Ochrona dostępu do poczty e-mail przed urządzeniami przy użyciu nowoczesnych klientów uwierzytelniania, takich jak program Outlook</span><span class="sxs-lookup"><span data-stu-id="c8b8a-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)