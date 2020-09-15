---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658888"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f6738-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f6738-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f6738-103">Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="f6738-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f6738-104">Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="f6738-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f6738-105">**Nie można zainstalować oprogramowania, 0x80cf4017:** Twój certyfikat konta wygasł.</span><span class="sxs-lookup"><span data-stu-id="f6738-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="f6738-106">Ponownie Pobierz pakiet oprogramowania klienckiego PC w konsoli administracyjnej usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="f6738-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="f6738-107">Aby uzyskać więcej informacji, zapoznaj się z tą dokumentacją.</span><span class="sxs-lookup"><span data-stu-id="f6738-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="f6738-108">**Kod błędu 0x801c0003:** Błąd może wystąpić w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="f6738-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="f6738-109">Użytkownik ma więcej urządzeń zarejestrowanych poza limitem urządzeń.</span><span class="sxs-lookup"><span data-stu-id="f6738-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f6738-110">Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f6738-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="f6738-111">"Użytkownicy mogą dołączać do urządzeń w usłudze Azure AD" ma ustawioną wartość "Brak".</span><span class="sxs-lookup"><span data-stu-id="f6738-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="f6738-112">Ustaw go na wszystkich lub wybierz pozycję Użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="f6738-112">Set it to all or select users.</span></span> <span data-ttu-id="f6738-113">Aby uzyskać więcej informacji, zapoznaj się z [tą dokumentacją](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="f6738-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="f6738-114">Urządzenie zostało już zarejestrowane przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f6738-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="f6738-115">W takim przypadku Usuń urządzenie z konsoli Azure Intune lub ręcznie odrejestrowania urządzenia przed ponowną próbą.</span><span class="sxs-lookup"><span data-stu-id="f6738-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="f6738-116">Urządzenie to Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="f6738-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="f6738-117">Do usługi Azure Active Directory można dołączyć tylko wersje Windows 10 Pro, Education i Enterprise.</span><span class="sxs-lookup"><span data-stu-id="f6738-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="f6738-118">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="f6738-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="f6738-119">Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="f6738-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f6738-120">Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.</span><span class="sxs-lookup"><span data-stu-id="f6738-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="f6738-121">Przejrzyj te dokumenty, aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie [problemów z](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)każdym z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) .</span><span class="sxs-lookup"><span data-stu-id="f6738-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="f6738-122">[Dowiedz się, jak zarejestrować urządzenia z systemem Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f6738-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
