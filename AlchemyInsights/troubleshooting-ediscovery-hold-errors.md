---
title: Rozwiązywanie problemów zbierania elektronicznych materiałów dowodowych zawiera błędy
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676278"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="5fb93-102">Rozwiązywanie problemów zbierania elektronicznych materiałów dowodowych zawiera błędy</span><span class="sxs-lookup"><span data-stu-id="5fb93-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="5fb93-103">Występują problemy z zbierania elektronicznych materiałów dowodowych?</span><span class="sxs-lookup"><span data-stu-id="5fb93-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="5fb93-104">Oto kilka najlepszych rozwiązań do rozważenia:</span><span class="sxs-lookup"><span data-stu-id="5fb93-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="5fb93-105">Sprawdź stan dystrybucji wstrzymaj.</span><span class="sxs-lookup"><span data-stu-id="5fb93-105">Check the hold distribution status.</span></span>  <span data-ttu-id="5fb93-106">Jeśli stan jest **Wł. (Oczekiwanie)** lub Wyłączony **(oczekiwanie),** poczekaj na zakończenie rozpowszechniania wstrzymywania.</span><span class="sxs-lookup"><span data-stu-id="5fb93-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="5fb93-107">Scal aktualizacje zbierania elektronicznych materiałów dowodowych w jedno żądanie zbiorcze, zamiast wielokrotnie aktualizować zasady dla każdej transakcji.</span><span class="sxs-lookup"><span data-stu-id="5fb93-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="5fb93-108">Uruchom Set-CaseHoldPolicy <policyname> -RetryDistribution w programie PowerShell Centrum zabezpieczeń i zgodności.</span><span class="sxs-lookup"><span data-stu-id="5fb93-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="5fb93-109">Aby uzyskać szczegółowe informacje, [Połączenie się z Centrum zabezpieczeń & w programie PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="5fb93-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="5fb93-110">Aby uzyskać instrukcje dotyczące sprawdzania tych ustawień i dodatkowych najlepszych rozwiązań związanych z ograniczaniem i rozwiązywaniem problemów dotyczących zbierania elektronicznych materiałów dowodowych, zobacz Rozwiązywanie problemów z błędami blokady zbierania [elektronicznych materiałów dowodowych.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="5fb93-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="5fb93-111">Aby uzyskać informacje na temat rozwiązywania innych typowych problemów zbierania elektronicznych materiałów dowodowych, zobacz Badanie, rozwiązywanie i rozwiązywanie typowych problemów [zbierania elektronicznych materiałów dowodowych.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="5fb93-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
