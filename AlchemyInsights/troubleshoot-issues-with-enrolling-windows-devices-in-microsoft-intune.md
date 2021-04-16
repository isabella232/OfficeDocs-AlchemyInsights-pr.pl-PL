---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808981"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="40b19-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Windows w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="40b19-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="40b19-103">Zapoznaj się z poniższymi zasobami, aby rozwiązać problem już teraz.</span><span class="sxs-lookup"><span data-stu-id="40b19-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="40b19-104">Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="40b19-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="40b19-105">**Oprogramowania nie można zainstalować, można 0x80cf4017:** Certyfikat konta wygasł.</span><span class="sxs-lookup"><span data-stu-id="40b19-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="40b19-106">Ponownie pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="40b19-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="40b19-107">Przejrzyj tę dokumentację, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="40b19-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="40b19-108">**Kod błędu 0x801c0003:** Błąd może występować w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="40b19-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="40b19-109">Zarejestrowanych urządzeń jest więcej niż wynosi limit urządzeń.</span><span class="sxs-lookup"><span data-stu-id="40b19-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="40b19-110">Przejrzyj te dokumenty, [aby usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub zmienić limit [urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="40b19-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="40b19-111">Wartość "Użytkownicy mogą dołączać do urządzeń w usłudze Azure AD" jest ustawiona na wartość "brak".</span><span class="sxs-lookup"><span data-stu-id="40b19-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="40b19-112">Ustaw ją na wszystkich lub wybranych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="40b19-112">Set it to all or select users.</span></span> <span data-ttu-id="40b19-113">Przejrzyj [tę dokumentację,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="40b19-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="40b19-114">Urządzenie zostało już zarejestrowane przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="40b19-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="40b19-115">W takim przypadku usuń urządzenie z konsoli usługi Azure Intune lub ręcznie wyeminuj urządzenie przed podjęciem próby po raz kolejny.</span><span class="sxs-lookup"><span data-stu-id="40b19-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="40b19-116">Urządzenie to Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="40b19-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="40b19-117">Tylko użytkownicy systemu Windows 10 Pro, Education i Enterprise mogą dołączyć do usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="40b19-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="40b19-118">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="40b19-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="40b19-119">Użyj [Portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="40b19-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="40b19-120">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="40b19-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="40b19-121">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrację i rozwiązanie dla każdego [z](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) nich: Przewodnik po rozwiązywaniu problemów i [Dokument rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="40b19-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="40b19-122">[Dowiedz się, jak zarejestrować urządzenia z systemem Windows w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="40b19-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
