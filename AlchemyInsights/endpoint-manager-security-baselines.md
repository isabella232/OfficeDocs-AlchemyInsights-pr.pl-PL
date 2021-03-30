---
title: Menedżer programu EndPoint — linie bazowe zabezpieczeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421086"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="bc05c-102">Menedżer programu EndPoint — linie bazowe zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="bc05c-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="bc05c-103">Linie bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, które ułatwiają stosowanie ustawień zabezpieczeń zalecanych przez odpowiednie zespoły ds. zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="bc05c-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="bc05c-104">Te linie bazowe można dostosować, aby dostarczyć tylko żądane ustawienia i wartości.</span><span class="sxs-lookup"><span data-stu-id="bc05c-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="bc05c-105">Aby uzyskać więcej informacji o planach bazowych zabezpieczeń, zobacz Konfigurowanie urządzeń z systemem [Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)w usłudze Intune przy użyciu planu bazowego zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="bc05c-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="bc05c-106">Obecnie istnieją linie bazowe dla tych produktów:</span><span class="sxs-lookup"><span data-stu-id="bc05c-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="bc05c-107">Ustawienia zabezpieczeń usługi Windows MDM</span><span class="sxs-lookup"><span data-stu-id="bc05c-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="bc05c-108">Program Microsoft Defender dla zabezpieczeń programu EndPoint</span><span class="sxs-lookup"><span data-stu-id="bc05c-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="bc05c-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bc05c-109">Microsoft Edge</span></span>

<span data-ttu-id="bc05c-110">Poszczególne linie bazowe są okresowo aktualizowane i zwalniane w wersjach przyrostowych.</span><span class="sxs-lookup"><span data-stu-id="bc05c-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="bc05c-111">Każda wersja dodaje i lub usuwa ustawienia z poprzedniej wersji, aby zapewnić, że plan bazowy spełnia bieżące wytyczne.</span><span class="sxs-lookup"><span data-stu-id="bc05c-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="bc05c-112">Konsola planu bazowego zabezpieczeń w zabezpieczeniach punktu końcowego umożliwia porównanie różnych wersji przez wprowadzenie zmian w poszczególnych wersjach.</span><span class="sxs-lookup"><span data-stu-id="bc05c-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="bc05c-113">Aby uzyskać wskazówki dotyczące najbardziej efektywnej zmiany wersji planu bazowego, zobacz Zarządzanie profilami planu bazowego zabezpieczeń w [usłudze Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="bc05c-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="bc05c-114">Po wdrożeniu planu bazowego zabezpieczeń możesz monitorować stan wdrożenia i przeglądać ustawienia w zależności od urządzenia.</span><span class="sxs-lookup"><span data-stu-id="bc05c-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="bc05c-115">**Uwaga:** Dane raportowania dla planu bazowego mogą być wyświetlane w ciągu 24 godzin od wdrożenie wstępne do urządzenia i do 6 godzin na dodatkowe aktualizacje.</span><span class="sxs-lookup"><span data-stu-id="bc05c-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="bc05c-116">Najczęstszą przyczyną nie zastosowania ustawienia planu bazowego jest to, że to samo ustawienie jest używane w innym profilu.</span><span class="sxs-lookup"><span data-stu-id="bc05c-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="bc05c-117">Ten scenariusz można zbadać dla określonego urządzenia, wybierając je w węźle Stan urządzenia profilu planu bazowego zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="bc05c-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="bc05c-118">Aby uzyskać szczegółowe informacje, zobacz [Rozwiązywanie konfliktów dotyczących planu bazowego zabezpieczeń.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="bc05c-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>