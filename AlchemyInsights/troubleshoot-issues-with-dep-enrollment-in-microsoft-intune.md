---
title: Rozwiązywanie problemów z rejestrowaniem funkcji DEP w usłudze Microsoft Intune
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
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797306"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="657b1-102">Rozwiązywanie problemów z rejestrowaniem funkcji DEP w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="657b1-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="657b1-103">Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="657b1-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="657b1-104">Jeśli urządzenie DEP nie może zarejestrować się, a uwierzytelnianie wieloskładnikowe (Multi-Factor Authentication) jest włączone, wyłącz funkcję MFA.</span><span class="sxs-lookup"><span data-stu-id="657b1-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="657b1-105">Obecnie funkcja MFA nie jest obsługiwana w przypadku rejestracji funkcji DEP</span><span class="sxs-lookup"><span data-stu-id="657b1-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="657b1-106">Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="657b1-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="657b1-107">Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.</span><span class="sxs-lookup"><span data-stu-id="657b1-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="657b1-108">Przejrzyj te dokumenty, aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie problemów z każdym z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="657b1-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="657b1-109">Informacje [o programie rejestracji urządzeń](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="657b1-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
