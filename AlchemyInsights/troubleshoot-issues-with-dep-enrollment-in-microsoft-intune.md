---
title: Rozwiązywanie problemów z rejestracją funkcji DEP w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 3e10f6729d760d9f8f6d04bcb33317fde51a9b80
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507029"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="bfe4c-102">Rozwiązywanie problemów z rejestracją funkcji DEP w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bfe4c-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="bfe4c-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="bfe4c-104">Jeśli funkcja DEP urządzenie jest w stanie zarejestrować i MFA (uwierzytelnianie wieloskładnikowe) jest włączone, należy wyłączyć MFA.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="bfe4c-105">Obecnie MFA nie jest obsługiwana w procesie rejestracji DEP</span><span class="sxs-lookup"><span data-stu-id="bfe4c-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="bfe4c-106">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bfe4c-107">Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="bfe4c-108">Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="bfe4c-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="bfe4c-109">[Więcej informacji na temat programu rejestracji urządzenia](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="bfe4c-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
