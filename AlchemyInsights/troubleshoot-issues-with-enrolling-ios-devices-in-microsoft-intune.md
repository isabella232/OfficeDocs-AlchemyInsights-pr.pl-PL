---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736168"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="dba03-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dba03-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="dba03-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="dba03-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="dba03-104">Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="dba03-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="dba03-105">**Osiągnięto limit urządzenia** Użytkownik ma więcej zarejestrowanych urządzeń niż limit urządzenia.</span><span class="sxs-lookup"><span data-stu-id="dba03-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="dba03-106">Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="dba03-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="dba03-107">**Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa apns (Apple Push Notification Service) musi być skonfigurowana lub odnowiona.</span><span class="sxs-lookup"><span data-stu-id="dba03-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="dba03-108">Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby uzyskać instrukcje, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="dba03-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="dba03-109">**Nieprawidłowy typ licencji użytkownika lub nazwa użytkownika nie została rozpoznana:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="dba03-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="dba03-110">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub Azure [portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="dba03-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="dba03-111">Dodatkowe zasoby ułatwiające rozwiązanie problemu:</span><span class="sxs-lookup"><span data-stu-id="dba03-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="dba03-112">Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="dba03-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="dba03-113">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="dba03-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="dba03-114">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązywanie problemów dla każdego z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [dokument rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="dba03-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="dba03-115">[Dowiedz się, jak rejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="dba03-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

