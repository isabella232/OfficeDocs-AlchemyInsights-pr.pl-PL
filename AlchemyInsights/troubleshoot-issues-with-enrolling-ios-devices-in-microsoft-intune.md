---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823473"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b86b2-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem iOS w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b86b2-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b86b2-103">Zapoznaj się z poniższymi zasobami, aby rozwiązać problem już teraz.</span><span class="sxs-lookup"><span data-stu-id="b86b2-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b86b2-104">Niektóre typowe komunikaty o błędach i procedury rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="b86b2-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b86b2-105">**Osiągnięto limit urządzeń** Zarejestrowanych urządzeń jest więcej niż wynosi limit urządzeń.</span><span class="sxs-lookup"><span data-stu-id="b86b2-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b86b2-106">Przejrzyj te dokumenty, [aby usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub zmienić limit [urządzeń](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b86b2-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b86b2-107">**Ta usługa nie jest obsługiwana. Bez zasad rejestracji:** Usługa wypychanych powiadomień (APNS) firmy Apple musi zostać skonfigurowana lub odnowiona.</span><span class="sxs-lookup"><span data-stu-id="b86b2-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="b86b2-108">Zapoznaj [się z tym dokumentem,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) aby dowiedzieć się, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="b86b2-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b86b2-109">**Typ licencji użytkownika Nieprawidłowy lub Nie rozpoznano nazwy użytkownika:** Użytkownikowi należy przypisać licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="b86b2-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b86b2-110">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: [Centrum administracyjnego pakietu Office](https://docs.microsoft.com/intune/licenses-assign) lub portalu Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="b86b2-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b86b2-111">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="b86b2-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b86b2-112">Użyj [Portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="b86b2-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b86b2-113">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="b86b2-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b86b2-114">Przejrzyj te dokumenty, aby uzyskać listę typowych błędów uniemożliwiających rejestrację i rozwiązanie dla każdego [z](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) nich: Przewodnik po rozwiązywaniu problemów i [Dokument rozwiązywania problemów.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b86b2-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b86b2-115">[Dowiedz się, jak zarejestrować urządzenia z systemem iOS w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="b86b2-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

