---
title: Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793894"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="e0ea8-102">Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="e0ea8-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="e0ea8-103">Linie bazowe zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="e0ea8-104">Plan bazowy zabezpieczeń Windows wstępnie skonfigurowane grupy używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="e0ea8-105">Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="e0ea8-106">Podczas wdrażania planu bazowego zabezpieczeń w grupach użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych Windows 10 lub nowszym.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="e0ea8-107">Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi firmy Microsoft automatycznie włącza funkcję funkcja BitLocker dla dysków wymiennych, wymaga hasła do odblokowania urządzenia i wyłącza uwierzytelnianie podstawowe.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="e0ea8-108">Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="e0ea8-109">Linie bazowe zabezpieczeń ułatwiają również utworzenie bezpiecznego, bezpiecznego przepływu pracy w Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="e0ea8-110">Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień wpływających na bezpieczeństwo.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="e0ea8-111">Usługa Intune współpracuje z zespołem zabezpieczeń Windows, który tworzy linie bazowe zasad grupy, więc te zalecenia są oparte na pełnych wskazówkach i obszernym doświadczeniu.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="e0ea8-112">Jeśli nie masz pewności, od czego zacząć, to plan bazowy zabezpieczeń pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil, jeśli nie masz pewności, od czego zacząć.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="e0ea8-113">Jeśli obecnie korzystasz z zasad grupy, migracja do usługi Intune do celów zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ są one wbudowane w usługę Intune i zawierają najnowe możliwości zarządzania.</span><span class="sxs-lookup"><span data-stu-id="e0ea8-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="e0ea8-114">Aby dowiedzieć się więcej, [zobacz Windows planu bazowego zabezpieczeń](/windows/security/threat-protection/windows-security-baselines) i Zarządzanie urządzeniami [przenośnymi.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="e0ea8-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

