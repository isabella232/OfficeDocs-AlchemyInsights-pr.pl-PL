---
title: Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planów bazowych zabezpieczeń usługi Microsoft Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573535"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="55cbb-102">Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planów bazowych zabezpieczeń usługi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="55cbb-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="55cbb-103">Plany bazowe dotyczące zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia.</span><span class="sxs-lookup"><span data-stu-id="55cbb-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="55cbb-104">Linie bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="55cbb-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="55cbb-105">Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, można utworzyć szablon składający się z wielu profilów konfiguracji urządzeń.</span><span class="sxs-lookup"><span data-stu-id="55cbb-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="55cbb-106">Podczas wdrażania planów bazowych zabezpieczeń do grup użytkowników lub urządzeń ustawienia są stosowane do urządzeń z systemem Windows 10 lub nowszym.</span><span class="sxs-lookup"><span data-stu-id="55cbb-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="55cbb-107">Na przykład linia bazowa zabezpieczeń oprogramowania MDM automatycznie (1) włącza funkcję BitLocker dla dysków wymiennych, (2) wymaga hasła do odblokowania urządzenia, a (3) wyłącza uwierzytelnianie podstawowe.</span><span class="sxs-lookup"><span data-stu-id="55cbb-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="55cbb-108">Jeśli wartość domyślna nie działa w danym środowisku, Dostosuj plan bazowy, aby zastosować potrzebne ustawienia.</span><span class="sxs-lookup"><span data-stu-id="55cbb-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="55cbb-109">Plany bazowe zabezpieczeń ułatwiają również ustanowienie bezpiecznego przepływu pracy w programie Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55cbb-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="55cbb-110">Poniżej przedstawiono niektóre zalety tego rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="55cbb-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="55cbb-111">Plan zabezpieczeń zawiera najważniejsze wskazówki i zalecenia dotyczące ustawień wpływających na bezpieczeństwo.</span><span class="sxs-lookup"><span data-stu-id="55cbb-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="55cbb-112">Ponieważ partnerzy usługi Intune z zespołem zabezpieczeń systemu Windows, który tworzy plany bazowe dla zasad grupy, te zalecenia są oparte na stałych wskazówkach i rozległych wrażeniach.</span><span class="sxs-lookup"><span data-stu-id="55cbb-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="55cbb-113">Jeśli nie znasz usługi Intune i nie wiesz, gdzie zacząć, punkty odniesienia w zabezpieczeniach ułatwią szybkie tworzenie i wdrażanie bezpiecznego profilu.</span><span class="sxs-lookup"><span data-stu-id="55cbb-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="55cbb-114">Jeśli obecnie korzystasz z zasad grupy, przeprowadzenie migracji do usługi Intune w celu zarządzania jest znacznie łatwiejsze w przypadku planów bezpieczeństwa, ponieważ są one wbudowane w usługę Intune i obejmują funkcje obcinania w celu zarządzania.</span><span class="sxs-lookup"><span data-stu-id="55cbb-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="55cbb-115">Aby dowiedzieć się więcej, zobacz [Plan bazowy zabezpieczeń systemu Windows](https://go.microsoft.com/fwlink/?linkid=2141503) i [Zarządzanie urządzeniami przenośnymi](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="55cbb-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>