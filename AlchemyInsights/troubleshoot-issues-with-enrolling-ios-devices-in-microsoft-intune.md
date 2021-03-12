---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708972"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="5ec14-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5ec14-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="5ec14-103">Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.</span><span class="sxs-lookup"><span data-stu-id="5ec14-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="5ec14-104">Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="5ec14-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="5ec14-105">**Osiągnięto limit urządzeń** Użytkownik ma zarejestrowanych więcej urządzeń niż wynosi limit urządzeń.</span><span class="sxs-lookup"><span data-stu-id="5ec14-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="5ec14-106">Przejrzyj te dokumenty, [aby usunąć urządzenie lub](https://docs.microsoft.com/intune/devices-wipe) zmienić limit [urządzeń.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="5ec14-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="5ec14-107">**Ta usługa nie jest obsługiwana. Bez zasad rejestracji:** usługa powiadomień push firmy Apple (APNS) wymaga skonfigurowania lub odnowienia.</span><span class="sxs-lookup"><span data-stu-id="5ec14-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="5ec14-108">Zapoznaj [się z tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby uzyskać instrukcje dotyczące tego, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="5ec14-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="5ec14-109">**Nieprawidłowy typ licencji użytkownika lub nie rozpoznano nazwy użytkownika:** Użytkownikowi musi być przypisana licencja usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="5ec14-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="5ec14-110">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Centrum administracyjnego pakietu Office](https://docs.microsoft.com/intune/licenses-assign) lub Portalu [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="5ec14-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="5ec14-111">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="5ec14-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5ec14-112">Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="5ec14-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5ec14-113">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="5ec14-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="5ec14-114">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrowanie i rozwiązywanie poszczególnych [problemów:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) przewodnik po rozwiązywaniu problemów i dokument [rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="5ec14-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="5ec14-115">[Dowiedz się, jak zarejestrować urządzenia z systemem iOS w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="5ec14-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

