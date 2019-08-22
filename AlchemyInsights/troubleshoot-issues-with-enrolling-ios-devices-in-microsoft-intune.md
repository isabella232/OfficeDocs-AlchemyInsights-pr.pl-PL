---
title: Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507013"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="5ab4c-102">Rozwiązywanie problemów z rejestrowanie urządzeń iOS w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5ab4c-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="5ab4c-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="5ab4c-104">Niektóre typowe komunikaty o błędach i kroki rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="5ab4c-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="5ab4c-105">**Cap urządzeń osiągnięty** Użytkownik ma więcej urządzeń zarejestrowanych niż limit urządzenia.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="5ab4c-106">Dokonują przeglądu tych dokumentów, aby [usunąć urządzenie](https://docs.microsoft.com/intune/devices-wipe) lub [zmienić limit urządzenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="5ab4c-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="5ab4c-107">**Ta usługa nie jest obsługiwana. Nie zasady rejestracji:** Apple Push powiadomień usługi (APN) musi być skonfigurowany lub odnowiony.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="5ab4c-108">Przegląd [Ten dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) instrukcje, jak to zrobić.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="5ab4c-109">**Nieprawidłowy typ licencji użytkownika ani nazwy użytkownika nie rozpoznany:** Użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="5ab4c-110">Dokonują przeglądu tych dokumentów przypisać jedną licencję do: [Witryna Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) lub [portalu Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="5ab4c-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="5ab4c-111">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="5ab4c-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5ab4c-112">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5ab4c-113">Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="5ab4c-114">Dokonują przeglądu tych dokumentów, listę typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego: [Podręcznik rozwiązywania problemów](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rozwiązywanie problemów doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="5ab4c-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="5ab4c-115">[Informacje o sposobie rejestrowania urządzeń iOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="5ab4c-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

