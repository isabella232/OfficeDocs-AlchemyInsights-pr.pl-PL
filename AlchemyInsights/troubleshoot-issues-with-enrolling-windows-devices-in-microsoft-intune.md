---
title: Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665842"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="22630-102">Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="22630-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="22630-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="22630-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="22630-104">Niektóre typowe komunikaty o błędach i kroki rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="22630-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="22630-105">**Nie można zainstalować oprogramowania, 0x80cf4017:** Twój certyfikat konta wygasło.</span><span class="sxs-lookup"><span data-stu-id="22630-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="22630-106">Ponownie Pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="22630-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="22630-107">Przejrzyj tę dokumentację, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="22630-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="22630-108">**Kod błędu 0x801c0003:** Ten błąd może wystąpić w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="22630-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="22630-109">Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia.</span><span class="sxs-lookup"><span data-stu-id="22630-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="22630-110">Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="22630-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="22630-111">"Użytkownicy mogą przyłączyć urządzenia do Azure AD" jest ustawiony na "Brak."</span><span class="sxs-lookup"><span data-stu-id="22630-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="22630-112">Ustaw go na wszystkie lub wybierz użytkowników.</span><span class="sxs-lookup"><span data-stu-id="22630-112">Set it to all or select users.</span></span> <span data-ttu-id="22630-113">Przegląd [tej dokumentacji](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="22630-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="22630-114">Urządzenie jest już zarejestrowane przez innego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="22630-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="22630-115">Jeśli tak się stanie, usuń urządzenie z konsoli Azure Intune lub ręcznie anulować rejestrację urządzenia przed ponowną próbą.</span><span class="sxs-lookup"><span data-stu-id="22630-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="22630-116">Urządzenie jest Windows 10 strona główna.</span><span class="sxs-lookup"><span data-stu-id="22630-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="22630-117">Tylko Windows 10 Pro, edukacji i wersji Enterprise można przyłączyć Azure usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="22630-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="22630-118">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="22630-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="22630-119">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="22630-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="22630-120">Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="22630-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="22630-121">Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="22630-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="22630-122">[Informacje o sposobie rejestrowania urządzeń systemu Windows w usłudze Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="22630-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
