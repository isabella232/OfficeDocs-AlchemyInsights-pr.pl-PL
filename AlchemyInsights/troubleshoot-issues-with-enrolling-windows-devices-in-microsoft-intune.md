---
title: Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482977"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0a663-102">Rozwiązywanie problemów z rejestrowania urządzenia z systemem Windows w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0a663-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0a663-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="0a663-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0a663-104">Niektóre typowe komunikaty o błędach i kroki rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="0a663-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0a663-p101">**Nie można zainstalować oprogramowania, 0x80cf4017:** Twój certyfikat konta wygasło. Ponownie Pobierz pakiet oprogramowania klienta komputera w konsoli administracyjnej usługi Intune. Przejrzyj tę dokumentację, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="0a663-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="0a663-108">**Kod błędu 0x801c0003:** Ten błąd może wystąpić w następujących scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="0a663-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="0a663-p102">Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia. Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/en-us/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0a663-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="0a663-p103">"Użytkownicy mogą przyłączyć urządzenia do Azure AD" jest ustawiony na "Brak". Ustaw go na wszystkie lub wybierz użytkowników. Przegląd [tej dokumentacji](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="0a663-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="0a663-p104">Urządzenie jest już zarejestrowane przez innego użytkownika. Jeśli tak się stanie, usuń urządzenie z konsoli Azure Intune lub ręcznie anulować rejestrację urządzenia przed ponowną próbą.</span><span class="sxs-lookup"><span data-stu-id="0a663-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="0a663-p105">Urządzenie jest Windows 10 strona główna. Tylko Windows 10 Pro, edukacji i wersji Enterprise można przyłączyć Azure usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a663-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="0a663-118">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="0a663-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0a663-p106">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="0a663-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0a663-121">Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0a663-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="0a663-122">[Informacje o sposobie rejestrowania urządzeń systemu Windows w usłudze Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="0a663-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

