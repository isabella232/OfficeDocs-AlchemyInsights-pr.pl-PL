---
title: Rozwiązywanie problemów z zapisaniem android w Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500081"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6fc7a-102">Rozwiązywanie problemów z zapisaniem android w Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6fc7a-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6fc7a-103">Przejrzyj zasoby wymienione poniżej, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6fc7a-104">Niektóre typowe problemy i czynności rozdzielczości:</span><span class="sxs-lookup"><span data-stu-id="6fc7a-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6fc7a-105">**Urządzenie nie zaszyfrowany błąd w portalu firmy:** Nowsze wersje Android, szczególnie począwszy od 7.0, wymagają podania hasła uruchamiania aby upewnić się, że urządzenie jest całkowicie zaszyfrowany.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="6fc7a-106">Aby włączyć numer pin uruchomienia lub urządzenie w pełni szyfrowania są wspólne rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="6fc7a-107">Przegląd [Ten dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="6fc7a-108">**Urządzeń nie powiedzie się sprawdzanie się przy użyciu usługi Windows Intune lub wyświetlić jako "Niezdrowego" w konsoli administracyjnej usługi Intune:** Niektóre firmy Samsung 4.4 i 5.5 urządzenia nie może sprawdzić w usłudze.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="6fc7a-109">Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="6fc7a-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="6fc7a-110">Ręcznie otworzyć aplikację Portal firmy Intune, który automatycznie rozpocznie synchronizowanie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="6fc7a-111">Aktualizowanie urządzenia do Android w wersji 6.0 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="6fc7a-112">Wyłączyć zarządzanie portalu Intune firmy Samsung Smart Menedżer.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="6fc7a-113">Przegląd [Ten dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , aby uzyskać szczegółowe informacje na temat te problemy i rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="6fc7a-114">**Nieprawidłowy typ licencji użytkownika** lub **użytkownika nazwa nie rozpoznany błąd:** użytkownik musi być przypisany licencji pakietu Windows Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6fc7a-115">Dokonują przeglądu tych dokumentów do przypisywania licencji za pomocą: portalu Office Admin Center lub Azure.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="6fc7a-116">Dodatkowe zasoby w celu rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="6fc7a-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6fc7a-117">Korzystać z [Portalu rozwiązywania problemów Windows Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6fc7a-118">Przegląd [tego dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="6fc7a-119">Przegląd [Ten dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) lista typowe błędy, które uniemożliwiają rejestracji i rozwiązania do każdego.</span><span class="sxs-lookup"><span data-stu-id="6fc7a-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="6fc7a-120">[Informacje o sposobie rejestrowania urządzeń Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="6fc7a-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
