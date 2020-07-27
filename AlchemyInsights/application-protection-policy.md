---
title: Zasady ochrony aplikacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423965"
---
# <a name="application-protection-policy"></a><span data-ttu-id="ca989-102">Zasady ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="ca989-102">Application protection policy</span></span>

<span data-ttu-id="ca989-103">Jeśli jesteś nowym użytkownikiem zasad ochrony aplikacji (APP), zapoznaj się z [omówieniem zasad ochrony aplikacji](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="ca989-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="ca989-104">Aby rozpocząć korzystanie z aplikacji, zobacz [Jak tworzyć i przypisywać zasady ochrony aplikacji](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="ca989-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="ca989-105">Wymagania dotyczące zasad ochrony aplikacji:</span><span class="sxs-lookup"><span data-stu-id="ca989-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="ca989-106">Użytkownik ma licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="ca989-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="ca989-107">Użytkownik należy do grupy, której dotyczy zasady ochrony aplikacji.</span><span class="sxs-lookup"><span data-stu-id="ca989-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="ca989-108">Tylko jeden użytkownik firmowy jest zalogowany do chronionych aplikacji na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="ca989-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="ca989-109">Aplikacja zaimplementowała [sdk usługi Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="ca989-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="ca989-110">Aby uzyskać listę aplikacji obsługujących pakiet SDK, zobacz [Aplikacje chronione usługi Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="ca989-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="ca989-111">Zasady mają zastosowanie po tym, jak użytkownik, który spełnia powyższe wymagania, zaloguje się do aplikacji obsługującej sdk usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="ca989-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="ca989-112">Najprostszym sposobem określenia, czy zasada jest stosowana, jest wymaganie, aby użytkownik ustawił pinezkę w zasadach.</span><span class="sxs-lookup"><span data-stu-id="ca989-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="ca989-113">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="ca989-113">For more information, see:</span></span>

[<span data-ttu-id="ca989-114">Często zadawane pytania dotyczące rozwiązywania problemów z aplikacją/mam</span><span class="sxs-lookup"><span data-stu-id="ca989-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="ca989-115">Jak sprawdzić poprawność konfiguracji zasad ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="ca989-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="ca989-116">Opis harmonogramu dostarczania zasad ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="ca989-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="ca989-117">Jak monitorować zasady ochrony aplikacji</span><span class="sxs-lookup"><span data-stu-id="ca989-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)