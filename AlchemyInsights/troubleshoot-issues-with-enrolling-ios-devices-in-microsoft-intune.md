---
title: Rozwiązywanie problemów z rejestrowanie urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507013"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="6a12a-102">Rozwiązywanie problemów z rejestrowanie urządzeń z systemem iOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6a12a-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="6a12a-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="6a12a-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="6a12a-104">Niektóre typowe komunikaty o błędach i kroki rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="6a12a-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="6a12a-105">**Osiągnięto limit urządzenia** Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia.</span><span class="sxs-lookup"><span data-stu-id="6a12a-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6a12a-106">Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="6a12a-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="6a12a-107">**Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa powiadomień wypychanych firmy Apple (APNS) musi być skonfigurowana lub odnawiana.</span><span class="sxs-lookup"><span data-stu-id="6a12a-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="6a12a-108">Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , aby uzyskać instrukcje, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="6a12a-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="6a12a-109">**Typ licencji użytkownika nieprawidłowy lub nie rozpoznano nazwy użytkownika:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="6a12a-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6a12a-110">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="6a12a-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="6a12a-111">Dodatkowe zasoby ułatwiające rozwiązanie problemu:</span><span class="sxs-lookup"><span data-stu-id="6a12a-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6a12a-112">Używaj [portalu rozwiązywania problemów z usługą Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) do diagnozowania i rozwiązywania typowych błędów rejestracji.</span><span class="sxs-lookup"><span data-stu-id="6a12a-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6a12a-113">Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="6a12a-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="6a12a-114">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów, które uniemożliwiają rejestrowanie i rozwiązania dla każdego: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [dokument dotyczący rozwiązywania problemów](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6a12a-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="6a12a-115">[Dowiedz się, jak rejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="6a12a-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

