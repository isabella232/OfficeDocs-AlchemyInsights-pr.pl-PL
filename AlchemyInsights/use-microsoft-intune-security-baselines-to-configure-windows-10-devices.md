---
title: Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planu bazowego zabezpieczeń usługi Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696377"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="06cb8-102">Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planu bazowego zabezpieczeń usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="06cb8-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="06cb8-103">Plan bazowy zabezpieczeń usługi Intune pomaga chronić użytkowników i urządzenia.</span><span class="sxs-lookup"><span data-stu-id="06cb8-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="06cb8-104">Plan bazowy zabezpieczeń to wstępnie skonfigurowane grupy systemu Windows służące do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły ds. zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="06cb8-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="06cb8-105">Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzenia.</span><span class="sxs-lookup"><span data-stu-id="06cb8-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="06cb8-106">Podczas wdrażania planu bazowego zabezpieczeń dla grup użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych w systemie Windows 10 lub nowszym.</span><span class="sxs-lookup"><span data-stu-id="06cb8-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="06cb8-107">Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi firmy Microsoft (MDM) automatycznie (1) włącza funkcję BitLocker dla dysków wymiennych, (2) wymaga hasła do odblokowania urządzenia, a (3) wyłącza uwierzytelnianie podstawowe.</span><span class="sxs-lookup"><span data-stu-id="06cb8-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="06cb8-108">Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.</span><span class="sxs-lookup"><span data-stu-id="06cb8-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="06cb8-109">Plan bazowy zabezpieczeń pomaga również w ustanawianiu end-to-end bezpiecznego przepływu pracy na platformy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="06cb8-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="06cb8-110">Oto niektóre z zalet tej funkcji:</span><span class="sxs-lookup"><span data-stu-id="06cb8-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="06cb8-111">Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień mających wpływ na bezpieczeństwo.</span><span class="sxs-lookup"><span data-stu-id="06cb8-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="06cb8-112">Ponieważ usługa Intune współpracuje z zespołem zabezpieczeń systemu Windows, który tworzy plan bazowy dla zasad grupy, te zalecenia są oparte na pełnych wskazówkach i obszernym doświadczeniu.</span><span class="sxs-lookup"><span data-stu-id="06cb8-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="06cb8-113">Jeśli nie masz pewności, od czego zacząć, nie wiesz, od czego zacząć, plan bazowy zabezpieczeń pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil.</span><span class="sxs-lookup"><span data-stu-id="06cb8-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="06cb8-114">Jeśli obecnie korzystasz z zasad grupy, migracja do intune w celu zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ te linie bazowe zabezpieczeń są wbudowane w usługę Intune i obejmują najnowodniej dostępne funkcje zarządzania.</span><span class="sxs-lookup"><span data-stu-id="06cb8-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="06cb8-115">Aby uzyskać więcej informacji, zobacz [plan bazowy zabezpieczeń systemu Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i zarządzanie urządzeniami [przenośnymi.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="06cb8-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>