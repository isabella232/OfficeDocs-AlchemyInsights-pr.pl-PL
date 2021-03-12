---
title: Rozwiązywanie problemów z rejestracją usługi DEP w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708720"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="9b8d6-102">Rozwiązywanie problemów z rejestracją usługi DEP w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9b8d6-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="9b8d6-103">Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.</span><span class="sxs-lookup"><span data-stu-id="9b8d6-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="9b8d6-104">Jeśli urządzenie funkcji DEP nie może zarejestrować się i uwierzytelnianie wieloskładnikowe jest włączone, wyłącz uwierzytelnianie wieloskładnikowe.</span><span class="sxs-lookup"><span data-stu-id="9b8d6-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="9b8d6-105">Obecnie uwierzytelniania wieloskładnikowego nie jest obsługiwane w przypadku rejestracji usługi DEP</span><span class="sxs-lookup"><span data-stu-id="9b8d6-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="9b8d6-106">Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="9b8d6-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9b8d6-107">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="9b8d6-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="9b8d6-108">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrowanie i rozwiązywanie poszczególnych [problemów:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) przewodnik po rozwiązywaniu problemów i dokument [rozwiązywania problemów](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="9b8d6-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="9b8d6-109">[Dowiedz się więcej o programie rejestracji urządzeń.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="9b8d6-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
