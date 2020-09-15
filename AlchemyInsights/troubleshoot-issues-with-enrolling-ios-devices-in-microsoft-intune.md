---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669258"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="97724-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="97724-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="97724-103">Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="97724-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="97724-104">Niektóre typowe komunikaty o błędach i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="97724-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="97724-105">**Osiągnięto koniec urządzenia** Użytkownik ma więcej urządzeń zarejestrowanych poza limitem urządzeń.</span><span class="sxs-lookup"><span data-stu-id="97724-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="97724-106">Przejrzyj te dokumenty, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="97724-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="97724-107">**Ta usługa nie jest obsługiwana. Brak zasad rejestracji:** usługa Apple Push Notification Service (APN) musi być skonfigurowana lub odnawiana.</span><span class="sxs-lookup"><span data-stu-id="97724-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="97724-108">Przejrzyj [ten dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , aby uzyskać instrukcje dotyczące wykonywania tej czynności.</span><span class="sxs-lookup"><span data-stu-id="97724-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="97724-109">**Typ licencji użytkownika jest nieprawidłowy lub nie rozpoznano nazwy użytkownika:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="97724-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="97724-110">Przejrzyj te dokumenty, aby przypisać licencję: [Centrum administracyjne pakietu Office](https://docs.microsoft.com/intune/licenses-assign) lub [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="97724-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="97724-111">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="97724-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="97724-112">Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="97724-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="97724-113">Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.</span><span class="sxs-lookup"><span data-stu-id="97724-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="97724-114">Przejrzyj te dokumenty, aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie [problemów z](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)każdym z nich: [Przewodnik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) .</span><span class="sxs-lookup"><span data-stu-id="97724-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="97724-115">[Dowiedz się, jak zarejestrować urządzenia z systemem iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="97724-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

