---
title: Dostęp warunkowy za pomocą usługi Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807669"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e7b8e-102">Dostęp warunkowy za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="e7b8e-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e7b8e-103">Używanie funkcji  **dostęp warunkowy**  z usługą Intune wymaga wykonania 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="e7b8e-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="e7b8e-104">Utwórz  **zasady zgodności**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e7b8e-105">Na przykład urządzenie musi mieć numer PIN o co najmniej 6 cyfrach, zanim zostanie uznany za zgodny.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="e7b8e-106">Utwórz **zasady dostępu warunkowego**  określające, jakie zasoby są chronione, a jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="e7b8e-107">[Na przykład](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  urządzenie musi być zgodne przed uzyskaniem dostępu do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="e7b8e-108">Upewnij się, że **zasady zgodności**  i  **zasady dostępu warunkowego**  są kierowane do żądanych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="e7b8e-109">Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7b8e-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="e7b8e-110">**Pomocne linki:**</span><span class="sxs-lookup"><span data-stu-id="e7b8e-110">**Helpful links:**</span></span>

[<span data-ttu-id="e7b8e-111">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="e7b8e-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="e7b8e-112">Rozwiązywanie problemów dotyczących urzędu certyfikacji</span><span class="sxs-lookup"><span data-stu-id="e7b8e-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e7b8e-113">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="e7b8e-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="e7b8e-114">Aby chronić wiadomości E-mail (usługi Exchange Online) przed dostępem za pomocą urządzeń niezgodnych, muszą być stosowane oba dokumenty:</span><span class="sxs-lookup"><span data-stu-id="e7b8e-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="e7b8e-115">Ochrona dostępu do poczty e-mail za pomocą urządzeń przy użyciu aplikacji EAS</span><span class="sxs-lookup"><span data-stu-id="e7b8e-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="e7b8e-116">Ochrona dostępu do poczty e-mail za pomocą urządzeń przy użyciu nowoczesnych klientów uwierzytelniania, takich jak program Outlook</span><span class="sxs-lookup"><span data-stu-id="e7b8e-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)