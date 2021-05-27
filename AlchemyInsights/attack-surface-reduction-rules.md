---
title: Reguły ograniczania powierzchni ataków
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676438"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c64ff-102">Reguły ograniczania powierzchni ataków</span><span class="sxs-lookup"><span data-stu-id="c64ff-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c64ff-103">Wykluczenie plików lub folderów może znacznie zmniejszyć ochronę zapewnianą przez reguły ograniczania powierzchni ataków.</span><span class="sxs-lookup"><span data-stu-id="c64ff-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c64ff-104">Pliki, które zostałyby zablokowane przez regułę, mogą być uruchamiane i nie są rejestrowane żadne raporty ani zdarzenia.</span><span class="sxs-lookup"><span data-stu-id="c64ff-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c64ff-105">Wszystkie reguły, które zezwalają na wykluczenia, mają zastosowanie wyłączenie.</span><span class="sxs-lookup"><span data-stu-id="c64ff-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c64ff-106">Wykluczenia asr mają taką samą składnię jak Program antywirusowy Microsoft Defender wykluczeń.</span><span class="sxs-lookup"><span data-stu-id="c64ff-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c64ff-107">Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie i weryfikowanie](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)wykluczeń Program antywirusowy Microsoft Defender skanowania.</span><span class="sxs-lookup"><span data-stu-id="c64ff-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c64ff-108">Aby uniknąć problemów, przejrzyj [typowe błędy, których można uniknąć podczas definiowania wykluczeń.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c64ff-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c64ff-109">Nie wszystkie reguły asr obsługują wykluczenia.</span><span class="sxs-lookup"><span data-stu-id="c64ff-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c64ff-110">Aby sprawdzić, czy reguła obsługuje wykluczenia, zobacz tabelę Reguły ograniczania powierzchni [ataków.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c64ff-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c64ff-111">Reguły ograniczania powierzchni ataków</span><span class="sxs-lookup"><span data-stu-id="c64ff-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c64ff-112">Miejsce ataków twojej organizacji obejmuje wszystkie miejsca, w których atakujący może naruszonć urządzenia lub sieci organizacji.</span><span class="sxs-lookup"><span data-stu-id="c64ff-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c64ff-113">Zmniejszenie powierzchni ataków oznacza ochronę urządzeń i sieci organizacji, co pozostawia atakującym mniej sposobów przeprowadzania ataków.</span><span class="sxs-lookup"><span data-stu-id="c64ff-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c64ff-114">Konfigurowanie reguł ograniczania powierzchni ataków w programie Microsoft Defender dla punktu końcowego może być pomocne.</span><span class="sxs-lookup"><span data-stu-id="c64ff-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c64ff-115">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="c64ff-115">For more information, see:</span></span>

- [<span data-ttu-id="c64ff-116">Mapuj identyfikator GUID reguły ASR na nazwę</span><span class="sxs-lookup"><span data-stu-id="c64ff-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c64ff-117">Wymagania dotyczące reguł asr:</span><span class="sxs-lookup"><span data-stu-id="c64ff-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c64ff-118">Windows 10 Pro, wersja 1709 lub nowsza</span><span class="sxs-lookup"><span data-stu-id="c64ff-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c64ff-119">Windows 10 Enterprise, wersja 1709 lub nowsza</span><span class="sxs-lookup"><span data-stu-id="c64ff-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c64ff-120">Windows Server, wersja 1803 (półroczny kanał) lub nowsza</span><span class="sxs-lookup"><span data-stu-id="c64ff-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c64ff-121">Określ prawidłowe wyłączenie, które ma być stosowane</span><span class="sxs-lookup"><span data-stu-id="c64ff-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c64ff-122">W dzienniku firmy Microsoft-Windows-Windows Defender/operacyjnym poszukaj Windows-1121 lub 1122.</span><span class="sxs-lookup"><span data-stu-id="c64ff-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c64ff-123">Oceń scenariusz blokowy i kontekst oraz potwierdź, że należy odblokować ten scenariusz.</span><span class="sxs-lookup"><span data-stu-id="c64ff-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c64ff-124">Odczytaj wartość Path (Ścieżka) w szczegółach zdarzenia, czyli wartość definiującą wykluczenie.</span><span class="sxs-lookup"><span data-stu-id="c64ff-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c64ff-125">Należy jak najsądniej o wyjątku.</span><span class="sxs-lookup"><span data-stu-id="c64ff-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c64ff-126">W razie potrzeby zastosuj symbol wieloznaczny (na przykład zamień zmienną użytkownika).</span><span class="sxs-lookup"><span data-stu-id="c64ff-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c64ff-127">Zastosuj wykluczenie zgodnie z potrzebami twojego wdrożenia.</span><span class="sxs-lookup"><span data-stu-id="c64ff-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c64ff-128">Aby uzyskać szczegółowe informacje, [zobacz Dostosowywanie reguł zmniejszania powierzchni ataków.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="c64ff-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c64ff-129">Wykluczenie nie jest honorowane</span><span class="sxs-lookup"><span data-stu-id="c64ff-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c64ff-130">Określanie, czy reguła obsługuje wykluczenia.</span><span class="sxs-lookup"><span data-stu-id="c64ff-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c64ff-131">Aby uzyskać szczegółowe informacje, [zobacz Reguły ograniczania powierzchni ataków.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c64ff-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c64ff-132">Przejrzyj zastosowane wykluczenia i sprawdź, czy dane zdarzeń nie mają literówek lub symboli wieloznacznych, które są nieprawidłowo interpretowane.</span><span class="sxs-lookup"><span data-stu-id="c64ff-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c64ff-133">Aby uzyskać więcej informacji, zobacz [Obsługiwane typy wykluczeń.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c64ff-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c64ff-134">jeśli wpływ reguły na tę regułę jest zbyt wysoki, rozważ przeniesienie (wstecz) reguły do trybu inspekcji w celu przeprowadzenia dalszych sprawdzania poprawności.</span><span class="sxs-lookup"><span data-stu-id="c64ff-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c64ff-135">Aby uzyskać szczegółowe informacje, zobacz Jak działają funkcje [programu Microsoft Defender dla punktu końcowego w trybie inspekcji.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="c64ff-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c64ff-136">Zbierz dane pomocy technicznej, aby otworzyć sprawę pomocy technicznej, używając tego polecenia:</span><span class="sxs-lookup"><span data-stu-id="c64ff-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c64ff-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c64ff-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c64ff-138">Aby uzyskać więcej informacji, zobacz [Problemy z komputerami dołączania do programu Microsoft Defender dla punktów końcowych.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="c64ff-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
