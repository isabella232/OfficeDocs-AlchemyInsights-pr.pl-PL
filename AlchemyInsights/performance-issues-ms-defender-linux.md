---
title: Problemy z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794002"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="17ab5-102">Problemy z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux</span><span class="sxs-lookup"><span data-stu-id="17ab5-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="17ab5-103">Ten artykuł przeprowadzi Cię przez kolejne etapy identyfikowania problemów z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux.</span><span class="sxs-lookup"><span data-stu-id="17ab5-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="17ab5-104">Najpierw należy sprawdzić, czy problem, który występuje, został rozwiązany za pomocą [najnowszej wersji](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="17ab5-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="17ab5-105">Aby rozpocząć badanie, zobacz Rozwiązywanie problemów z wydajnością [programu Microsoft Defender dla punktu końcowego w systemie Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="17ab5-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="17ab5-106">Wykluczenia</span><span class="sxs-lookup"><span data-stu-id="17ab5-106">Exclusions</span></span>

<span data-ttu-id="17ab5-107">Wykluczenia mogą pomóc zminimalizować problemy z wydajnością.</span><span class="sxs-lookup"><span data-stu-id="17ab5-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="17ab5-108">Przed rozpoczęciem przejrzyj swoje wykluczenia, aby sprawdzić i udokumentować wszelkie dodatkowe zagrożenia.</span><span class="sxs-lookup"><span data-stu-id="17ab5-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="17ab5-109">Aby uzyskać więcej informacji, zobacz Konfigurowanie i weryfikowanie wykluczeń programu [Microsoft Defender dla punktu końcowego w systemie Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="17ab5-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="17ab5-110">Jeśli masz wiele plików, & wykluczyć, a wszystkie są w tym samym punkcie instalacji, łatwiej będzie wykluczyć punkt instalacji.</span><span class="sxs-lookup"><span data-stu-id="17ab5-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="17ab5-111">Od lutego w wersji 101.22.80 można wykluczyć cały punkt instalacji.</span><span class="sxs-lookup"><span data-stu-id="17ab5-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="17ab5-112">Jeśli na przykład /mnt/backup jest punktem instalacji, możesz dodać polecenie /mnt/backup do listy wykluczeń, uruchamiając to polecenie:</span><span class="sxs-lookup"><span data-stu-id="17ab5-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="17ab5-113">**Uwaga:** Dodanie wykluczeń zwiększa ryzyko, że złośliwe oprogramowanie nie jest wykrywane, a jego obsługa i wdrożenie należy zachować ostrożność.</span><span class="sxs-lookup"><span data-stu-id="17ab5-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="17ab5-114">Potrzebujesz pomocy?</span><span class="sxs-lookup"><span data-stu-id="17ab5-114">Need Help?</span></span>

<span data-ttu-id="17ab5-115">Aby pomóc w najskuteczniejszy sposób, zbierz dane diagnostyczne przed otwarciem sprawy pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="17ab5-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
