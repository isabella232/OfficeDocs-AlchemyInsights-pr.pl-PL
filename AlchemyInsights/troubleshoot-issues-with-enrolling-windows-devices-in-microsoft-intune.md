---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708900"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="45612-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="45612-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="45612-103">Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.</span><span class="sxs-lookup"><span data-stu-id="45612-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="45612-104">Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="45612-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="45612-105">**Nie można zainstalować oprogramowania, 0x80cf4017:** Certyfikat konta wygasł.</span><span class="sxs-lookup"><span data-stu-id="45612-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="45612-106">Ponownie pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="45612-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="45612-107">Aby uzyskać więcej informacji, zapoznaj się z tą dokumentacją.</span><span class="sxs-lookup"><span data-stu-id="45612-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="45612-108">**Kod błędu 0x801c0003:** Błąd może występować w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="45612-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="45612-109">Użytkownik ma zarejestrowanych więcej urządzeń niż wynosi limit urządzeń.</span><span class="sxs-lookup"><span data-stu-id="45612-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="45612-110">Przejrzyj te dokumenty, [aby usunąć urządzenie lub](https://docs.microsoft.com/intune/devices-wipe) zmienić limit [urządzeń.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="45612-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="45612-111">Ustawienie "Użytkownicy mogą dołączać urządzenia do usługi Azure AD" ma wartość "brak".</span><span class="sxs-lookup"><span data-stu-id="45612-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="45612-112">Ustaw ją na wszystkich lub wybierz użytkowników.</span><span class="sxs-lookup"><span data-stu-id="45612-112">Set it to all or select users.</span></span> <span data-ttu-id="45612-113">Aby [uzyskać więcej informacji,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) zapoznaj się z tą dokumentacją.</span><span class="sxs-lookup"><span data-stu-id="45612-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="45612-114">Urządzenie zostało już zarejestrowane przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="45612-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="45612-115">W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie usuń je przed podjęciem próby.</span><span class="sxs-lookup"><span data-stu-id="45612-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="45612-116">Urządzenie to Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="45612-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="45612-117">Do usługi Azure Active Directory mogą dołączyć tylko jednostki SKU systemu Windows 10 Pro, Education i Enterprise.</span><span class="sxs-lookup"><span data-stu-id="45612-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="45612-118">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="45612-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="45612-119">Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="45612-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="45612-120">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="45612-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="45612-121">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrowanie i rozwiązywanie poszczególnych [problemów:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) przewodnik po rozwiązywaniu problemów i dokument [rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="45612-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="45612-122">[Dowiedz się, jak zarejestrować urządzenia z systemem Windows w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="45612-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
