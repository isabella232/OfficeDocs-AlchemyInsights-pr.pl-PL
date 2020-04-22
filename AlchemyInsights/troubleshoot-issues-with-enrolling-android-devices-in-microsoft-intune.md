---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759630"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="604ad-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="604ad-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="604ad-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="604ad-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="604ad-104">Niektóre typowe problemy i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="604ad-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="604ad-105">**Błąd nieszyfrowany na urządzeniu w portalu firmy:** Nowsze wersje systemu Android, szczególnie począwszy od wersji 7.0, wymagają kodu startowego, aby upewnić się, że urządzenie jest w pełni zaszyfrowane.</span><span class="sxs-lookup"><span data-stu-id="604ad-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="604ad-106">Typowe rozwiązania mają na celu włączenie numeru pinstart lub pełne zaszyfrowanie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="604ad-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="604ad-107">Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="604ad-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="604ad-108">**Urządzenia nie mogą zaewidencjonować usługi Intune lub wyświetlić jako "w złej kondycji" w konsoli administracyjnej usługi Intune:** Niektóre urządzenia Samsung 4.4 i 5.5 mogą nie zameldowyw przypadku usługi.</span><span class="sxs-lookup"><span data-stu-id="604ad-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="604ad-109">Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="604ad-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="604ad-110">Ręcznie otwórz aplikację Portal firmy usługi Intune, która automatycznie zainicjuje synchronizację urządzenia.</span><span class="sxs-lookup"><span data-stu-id="604ad-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="604ad-111">Zaktualizuj urządzenie do systemu Android 6.0 lub nowszego.</span><span class="sxs-lookup"><span data-stu-id="604ad-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="604ad-112">Wyłącz program Samsung Smart Manager z zarządzania portalem firmy usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="604ad-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="604ad-113">Zapoznaj się z [tym dokumentem,](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) aby uzyskać więcej informacji na temat tych problemów i rozwiązań.</span><span class="sxs-lookup"><span data-stu-id="604ad-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="604ad-114">**Nieprawidłowy typ licencji użytkownika** lub **błąd Nieuznany użytkownik:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="604ad-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="604ad-115">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: Centrum administracyjne pakietu Office lub witryny Azure portal.</span><span class="sxs-lookup"><span data-stu-id="604ad-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="604ad-116">Dodatkowe zasoby ułatwiające rozwiązanie problemu:</span><span class="sxs-lookup"><span data-stu-id="604ad-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="604ad-117">Użyj [portalu rozwiązywania problemów z usługi Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="604ad-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="604ad-118">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="604ad-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="604ad-119">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązania dla każdego z nich.</span><span class="sxs-lookup"><span data-stu-id="604ad-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="604ad-120">[Dowiedz się, jak rejestrować urządzenia z systemem Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="604ad-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
