---
title: Endpoint Manager — Plany bazowe zabezpieczeń
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440894"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="8a85d-102">Endpoint Manager — Plany bazowe zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="8a85d-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="8a85d-103">Plany bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, które ułatwiają stosowanie ustawień zabezpieczeń zalecanych przez odpowiednie zespoły ds. zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="8a85d-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="8a85d-104">Te plany bazowe można dostosować tak, aby zawierały tylko wymagane ustawienia i wartości.</span><span class="sxs-lookup"><span data-stu-id="8a85d-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="8a85d-105">Aby uzyskać więcej informacji o planach bazowych zabezpieczeń, zobacz [Używanie planów bazowych zabezpieczeń do konfigurowania urządzeń z systemem Windows 10 w usłudze Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="8a85d-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="8a85d-106">Obecnie są dostępne plany bazowe dla tych produktów:</span><span class="sxs-lookup"><span data-stu-id="8a85d-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="8a85d-107">Ustawienia zabezpieczeń funkcji zarządzania urządzeniami przenośnymi z systemem Windows</span><span class="sxs-lookup"><span data-stu-id="8a85d-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="8a85d-108">Zabezpieczenia usługi Ochrona punktu końcowego w usłudze Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="8a85d-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="8a85d-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8a85d-109">Microsoft Edge</span></span>

<span data-ttu-id="8a85d-110">Wszystkie plany bazowe są okresowo aktualizowane i wydawane w wersjach przyrostowych.</span><span class="sxs-lookup"><span data-stu-id="8a85d-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="8a85d-111">Każda wersja dodaje ustawienia do poprzedniej wersji lub usuwa je z niej, aby zapewnić, że plan bazowy spełnia bieżące wytyczne.</span><span class="sxs-lookup"><span data-stu-id="8a85d-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="8a85d-112">Konsola planów bazowych zabezpieczeń w zabezpieczeniach punktów końcowych umożliwia porównanie różnych wersji przez uwidocznienie zmian wprowadzanych w poszczególnych wersjach.</span><span class="sxs-lookup"><span data-stu-id="8a85d-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="8a85d-113">Aby uzyskać wskazówki dotyczące najskuteczniejszego zmieniania wersji wdrożonego planu bazowego, zobacz [Zarządzanie profilami planu bazowego zabezpieczeń w usłudze Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="8a85d-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="8a85d-114">Po wdrożeniu planu bazowego zabezpieczeń możesz monitorować stan wdrożenia i przeglądać ustawienia na poszczególnych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="8a85d-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="8a85d-115">**Uwaga:** Zanim dane raportowania dla planów bazowych będą widoczne, od momentu wdrożenia wstępnego na urządzeniu może upłynąć do 24 godzin, a w przypadku kolejnych aktualizacji do 6 godzin.</span><span class="sxs-lookup"><span data-stu-id="8a85d-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="8a85d-116">Najczęstszą przyczyną niezastosowania ustawienia planu bazowego jest to, że to samo ustawienie jest używane w innym profilu.</span><span class="sxs-lookup"><span data-stu-id="8a85d-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="8a85d-117">Ten scenariusz można zbadać dla konkretnego urządzenia, wybierając to urządzenie w węźle Stan urządzenia profilu planu bazowego zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="8a85d-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="8a85d-118">Aby uzyskać szczegółowe informacje, zobacz [Rozwiązywanie konfliktów dotyczących planów bazowych zabezpieczeń](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="8a85d-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>