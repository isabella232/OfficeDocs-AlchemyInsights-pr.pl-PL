---
title: Błędy synchronizacji automatycznego rejestrowania urządzeń firmy Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714828"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="72704-102">Błędy synchronizacji automatycznego rejestrowania urządzeń firmy Apple</span><span class="sxs-lookup"><span data-stu-id="72704-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="72704-103">"Wykryto, że masz co najmniej jeden token ADE/DEP w stanie błędu.</span><span class="sxs-lookup"><span data-stu-id="72704-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="72704-104">Do momentu rozwiązania błędu w odniesieniu do każdego z tokenów, których dotyczy problem, funkcja ADE nie będzie działać w przypadku tego samego ".</span><span class="sxs-lookup"><span data-stu-id="72704-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="72704-105">Ten błąd może być manifestem na kilka sposobów, takich jak:</span><span class="sxs-lookup"><span data-stu-id="72704-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="72704-106">Urządzenia mogą nie być synchronizowane z ABM/ASM do usługi Intune</span><span class="sxs-lookup"><span data-stu-id="72704-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="72704-107">Zadania profilu rejestracji mogą być błędne</span><span class="sxs-lookup"><span data-stu-id="72704-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="72704-108">Urządzenia mogą nie zakończyć się pomyślnie rejestracji w programie ADE</span><span class="sxs-lookup"><span data-stu-id="72704-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="72704-109">Sprawdź, czy w konsoli usługi Intune Wystąpił błąd synchronizacji w obszarze **urządzenia > zarejestrować urządzenia > rejestracji firmy Apple > tokeny programu rejestracji** i zapoznaj się z poniższą dokumentacją w celu wyświetlenia ewentualnych środków zaradczych:</span><span class="sxs-lookup"><span data-stu-id="72704-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="72704-110">Błędy synchronizacji ABM/ASM dla tokenów automatycznego rejestrowania urządzeń z systemami iOS/iPadOS i macOS</span><span class="sxs-lookup"><span data-stu-id="72704-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
