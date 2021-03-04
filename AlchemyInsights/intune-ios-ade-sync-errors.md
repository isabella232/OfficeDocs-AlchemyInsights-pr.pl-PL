---
title: Błędy synchronizacji automatycznej rejestracji urządzeń firmy Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448932"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="6b692-102">Błędy synchronizacji automatycznej rejestracji urządzeń firmy Apple</span><span class="sxs-lookup"><span data-stu-id="6b692-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="6b692-103">"Wykryliśmy, że masz co najmniej jeden token ADE/DEP, które znajdują się w stanie błędu.</span><span class="sxs-lookup"><span data-stu-id="6b692-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="6b692-104">Do czasu rozwiązania stanu błędu dla każdego tokenu, którego dotyczy problem, funkcja ADE nie będzie działać zgodnie z oczekiwaniami".</span><span class="sxs-lookup"><span data-stu-id="6b692-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="6b692-105">Ten błąd może wystąpić na wiele sposobów, takich jak:</span><span class="sxs-lookup"><span data-stu-id="6b692-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="6b692-106">Urządzenia mogą nie być synchronizowane z abm/asm w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="6b692-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="6b692-107">Przypisania profilów rejestracji mogą się nie pomylić</span><span class="sxs-lookup"><span data-stu-id="6b692-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="6b692-108">Urządzenia mogą nie ukończyć pomyślnie rejestracji ADE</span><span class="sxs-lookup"><span data-stu-id="6b692-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="6b692-109">Sprawdź, czy nie wystąpił błąd synchronizacji zgłoszony w konsoli Intune w obszarze Urządzenia > Zarejestruj urządzenia > rejestracji firmy Apple > **tokenów programu rejestracji.**</span><span class="sxs-lookup"><span data-stu-id="6b692-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="6b692-110">Jedną z najbardziej typowych przyczyn błędu synchronizacji jest wygaśnięcie bieżącego tokenu.</span><span class="sxs-lookup"><span data-stu-id="6b692-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="6b692-111">W wielu przypadkach odnowienie tokenu, którego dotyczy problem, rozwiąże ten problem.</span><span class="sxs-lookup"><span data-stu-id="6b692-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="6b692-112">Jeśli co najmniej jeden z Twoich tokenów wygasł, zapoznaj się z następującą dokumentacją, aby ułatwić odnawianie ich w razie potrzeby:</span><span class="sxs-lookup"><span data-stu-id="6b692-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="6b692-113">Odnawianie tokenu automatycznej rejestracji urządzenia</span><span class="sxs-lookup"><span data-stu-id="6b692-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="6b692-114">Ponadto możesz zobaczyć następującą dokumentację, aby zobaczyć potencjalne działania naprawcze dotyczące innych błędów powodujących błędy synchronizacji tokenów:</span><span class="sxs-lookup"><span data-stu-id="6b692-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="6b692-115">Błędy synchronizacji ABM/ASM dla tokenów automatycznej rejestracji urządzeń dla systemów iOS/iPadOS i macOS</span><span class="sxs-lookup"><span data-stu-id="6b692-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="6b692-116">Błędy synchronizacji ABM/ASM dla tokenów automatycznej rejestracji urządzeń dla systemów iOS/iPadOS i macOS</span><span class="sxs-lookup"><span data-stu-id="6b692-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
