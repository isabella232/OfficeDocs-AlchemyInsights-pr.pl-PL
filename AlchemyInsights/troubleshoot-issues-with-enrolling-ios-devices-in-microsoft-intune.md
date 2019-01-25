---
title: Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483265"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="a4e4e-102">Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a4e4e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="a4e4e-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="a4e4e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="a4e4e-104">Niektóre typowe komunikaty o błędach i kroki rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="a4e4e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="a4e4e-p101">**Cap urządzeń osiągnięty** Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia. Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/en-us/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a4e4e-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="a4e4e-p102">**Ta usługa nie jest obsługiwana. Nie zasady rejestracji:** Apple Push powiadomień usługi (APN) musi być skonfigurowany lub odnowiony. Przegląd [Ten dokument](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) instrukcje, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="a4e4e-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="a4e4e-p103">**Nieprawidłowy typ licencji użytkownika ani nazwy użytkownika nie rozpoznany:** Użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS. Dokonują przeglądu tych dokumentów przypisać jedną licencję do: [Witryna Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) lub [portalu Azure](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="a4e4e-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="a4e4e-111">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="a4e4e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a4e4e-p104">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="a4e4e-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a4e4e-114">Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a4e4e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="a4e4e-115">[Informacje o sposobie rejestrowania urządzeń iOS w usłudze Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="a4e4e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

