---
title: Rozwiązywanie problemów z zapisaniem android w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28305106"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="de391-102">Rozwiązywanie problemów z zapisaniem android w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="de391-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="de391-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="de391-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="de391-104">Niektóre typowe problemy i czynności rozdzielczości:</span><span class="sxs-lookup"><span data-stu-id="de391-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="de391-p101">**Urządzenie nie zaszyfrowany błąd w portalu firmy:** Nowsze wersje Android, szczególnie począwszy od 7.0, wymagają podania hasła uruchamiania aby upewnić się, że urządzenie jest całkowicie zaszyfrowany. Aby włączyć numer pin uruchomienia lub urządzenie w pełni szyfrowania są wspólne rozwiązania. Przegląd [Ten dokument](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="de391-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="de391-p102">**Urządzeń nie powiedzie się sprawdzanie się przy użyciu usługi Windows Intune lub wyświetlić jako "Niezdrowego" w konsoli administracyjnej usługi Intune:** Niektóre firmy Samsung 4.4 i 5.5 urządzenia nie może sprawdzić w usłudze. Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="de391-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="de391-110">Ręcznie otworzyć aplikację Portal firmy Intune, który automatycznie rozpocznie synchronizowanie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="de391-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="de391-111">Aktualizowanie urządzenia do Android w wersji 6.0 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="de391-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="de391-p103">Wyłączyć zarządzanie portalu Intune firmy Samsung Smart Menedżer. Przegląd [Ten dokument](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , aby uzyskać szczegółowe informacje na temat te problemy i rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="de391-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="de391-p104">**Nieprawidłowy typ licencji użytkownika** lub **użytkownika nazwa nie rozpoznany błąd:** użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS. Dokonują przeglądu tych dokumentów do przypisywania licencji za pomocą: portalu Office Admin Center lub Azure.</span><span class="sxs-lookup"><span data-stu-id="de391-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="de391-116">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="de391-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="de391-p105">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji. Przegląd [tego dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="de391-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="de391-119">Przegląd [Ten dokument](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) lista typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego.</span><span class="sxs-lookup"><span data-stu-id="de391-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="de391-120">[Informacje o sposobie rejestrowania urządzeń Android w usłudze Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="de391-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

