---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665842"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="89bfc-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="89bfc-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="89bfc-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="89bfc-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="89bfc-104">Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="89bfc-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="89bfc-105">**Nie można zainstalować oprogramowania, 0x80cf4017:** Certyfikat konta wygasł.</span><span class="sxs-lookup"><span data-stu-id="89bfc-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="89bfc-106">Pobierz ponownie pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="89bfc-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="89bfc-107">Zapoznaj się z tą dokumentacją, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="89bfc-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="89bfc-108">**Kod błędu 0x801c0003:** Błąd może wystąpić w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="89bfc-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="89bfc-109">Użytkownik ma więcej zarejestrowanych urządzeń niż limit urządzenia.</span><span class="sxs-lookup"><span data-stu-id="89bfc-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="89bfc-110">Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="89bfc-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="89bfc-111">"Użytkownicy mogą dołączyć do urządzeń do usługi Azure AD" jest ustawiona na "brak".</span><span class="sxs-lookup"><span data-stu-id="89bfc-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="89bfc-112">Ustaw go na wszystkich lub wybierz użytkowników.</span><span class="sxs-lookup"><span data-stu-id="89bfc-112">Set it to all or select users.</span></span> <span data-ttu-id="89bfc-113">Zapoznaj się z [tą dokumentacją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="89bfc-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="89bfc-114">Urządzenie jest już zarejestrowane przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="89bfc-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="89bfc-115">W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie wyrejestruj urządzenie przed ponowną próbą.</span><span class="sxs-lookup"><span data-stu-id="89bfc-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="89bfc-116">Urządzenie jest Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="89bfc-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="89bfc-117">Tylko jednostki SKU systemu Windows 10 Pro, Education i Enterprise mogą dołączyć do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89bfc-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="89bfc-118">Dodatkowe zasoby ułatwiające rozwiązanie problemu:</span><span class="sxs-lookup"><span data-stu-id="89bfc-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="89bfc-119">Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="89bfc-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="89bfc-120">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="89bfc-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="89bfc-121">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązywanie problemów dla każdego z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [dokument rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="89bfc-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="89bfc-122">[Dowiedz się, jak rejestrować urządzenia z systemem Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="89bfc-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
