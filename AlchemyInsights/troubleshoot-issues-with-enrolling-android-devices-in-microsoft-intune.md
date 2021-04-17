---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830952"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9bced-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9bced-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9bced-103">Zapoznaj się z poniższymi zasobami, aby rozwiązać problem już teraz.</span><span class="sxs-lookup"><span data-stu-id="9bced-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9bced-104">Niektóre typowe problemy i kroki rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="9bced-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9bced-105">**Błąd urządzenia nie szyfrowanego w portalu firmy:** Nowsze wersje systemu Android, zwłaszcza począwszy od wersji 7.0, wymagają kodu dostępu podczas uruchamiania, aby upewnić się, że urządzenie jest w pełni zaszyfrowane.</span><span class="sxs-lookup"><span data-stu-id="9bced-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="9bced-106">Typowe rozwiązania to włączenie numeru PIN startowego lub pełne zaszyfrowanie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="9bced-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="9bced-107">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="9bced-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="9bced-108">Urządzenia nie mogą sprawdzić się za pomocą usługi Intune lub są **wyświetlane jako "Zła" w konsoli administracyjnej Intune:** Niektóre urządzenia z systemem Samsung 4.4 i 5.5 mogą nie sprawdzić się w usłudze.</span><span class="sxs-lookup"><span data-stu-id="9bced-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="9bced-109">Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="9bced-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="9bced-110">Ręcznie otwórz aplikację Portalu firmy Intune, która automatycznie zainicjuje synchronizację urządzenia.</span><span class="sxs-lookup"><span data-stu-id="9bced-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="9bced-111">Zaktualizuj urządzenie do wersji Android 6.0 lub wyższej.</span><span class="sxs-lookup"><span data-stu-id="9bced-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="9bced-112">Wyłącz funkcję Samsung Smart Manager z zarządzania portalem firmy Intune.</span><span class="sxs-lookup"><span data-stu-id="9bced-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="9bced-113">Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) aby uzyskać szczegółowe informacje na temat tych problemów i ich rozwiązywania.</span><span class="sxs-lookup"><span data-stu-id="9bced-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="9bced-114">**Błąd Nieprawidłowe typy licencji** użytkownika lub Nazwa użytkownika nie **rozpoznano:** Użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="9bced-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9bced-115">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: Centrum administracyjnego pakietu Office lub portalu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9bced-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="9bced-116">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="9bced-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9bced-117">Użyj [Portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="9bced-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9bced-118">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="9bced-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9bced-119">Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązanie dla każdego z nich.</span><span class="sxs-lookup"><span data-stu-id="9bced-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="9bced-120">[Dowiedz się, jak zarejestrować urządzenia z systemem Android w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="9bced-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
