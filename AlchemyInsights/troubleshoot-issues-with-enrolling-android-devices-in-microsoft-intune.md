---
title: Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709008"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="2fa86-102">Rozwiązywanie problemów z zarejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2fa86-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="2fa86-103">Przejrzyj zasoby wymienione poniżej, aby teraz rozwiązać problem.</span><span class="sxs-lookup"><span data-stu-id="2fa86-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2fa86-104">Niektóre typowe problemy i procedury rozwiązywania problemów:</span><span class="sxs-lookup"><span data-stu-id="2fa86-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="2fa86-105">**Błąd urządzenia, który nie jest zaszyfrowany w portalu firmy:** Nowsze wersje systemu Android, zwłaszcza począwszy od wersji 7.0, wymagają kodu dostępu podczas uruchamiania, aby upewnić się, że urządzenie jest w pełni zaszyfrowane.</span><span class="sxs-lookup"><span data-stu-id="2fa86-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="2fa86-106">Typowe rozwiązania to włączenie numeru PIN startowego lub pełne zaszyfrowanie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="2fa86-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="2fa86-107">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="2fa86-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="2fa86-108">Urządzenia nie mogą się sprawdzić za pomocą usługi Intune lub są wyświetlane jako **"Zła kondycja" w konsoli administracyjnej Intune:** Niektóre urządzenia z systemem Samsung 4.4 i 5.5 mogą nie sprawdzić się w usłudze.</span><span class="sxs-lookup"><span data-stu-id="2fa86-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="2fa86-109">Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="2fa86-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="2fa86-110">Ręcznie otwórz aplikację portalu firmy Intune, która automatycznie zainicjuje synchronizację urządzeń.</span><span class="sxs-lookup"><span data-stu-id="2fa86-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="2fa86-111">Zaktualizuj urządzenie do wersji Android 6.0 lub wyższej.</span><span class="sxs-lookup"><span data-stu-id="2fa86-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="2fa86-112">Wyłącz funkcję Samsung Smart Manager z zarządzania portalem firmy Intune.</span><span class="sxs-lookup"><span data-stu-id="2fa86-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="2fa86-113">Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) aby uzyskać szczegółowe informacje na temat tych problemów i ich rozwiązywania.</span><span class="sxs-lookup"><span data-stu-id="2fa86-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="2fa86-114">**Błąd "Nieprawidłowy typ** licencji użytkownika" lub "Nazwa użytkownika nie rozpoznano": użytkownikowi należy przypisać licencję usługi Intune lub EMS. </span><span class="sxs-lookup"><span data-stu-id="2fa86-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2fa86-115">Przejrzyj te dokumenty, aby przypisać licencję za pośrednictwem: Centrum administracyjnego pakietu Office lub Portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="2fa86-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="2fa86-116">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="2fa86-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2fa86-117">Użyj [portalu rozwiązywania problemów Intune,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="2fa86-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2fa86-118">Przejrzyj [ten dokument,](https://docs.microsoft.com/intune/help-desk-operators) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="2fa86-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="2fa86-119">Przejrzyj [ten dokument,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) aby uzyskać listę typowych błędów, które uniemożliwiają rejestrację i rozwiązanie każdego z nich.</span><span class="sxs-lookup"><span data-stu-id="2fa86-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="2fa86-120">[Dowiedz się, jak zarejestrować urządzenia z systemem Android w usłudze Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="2fa86-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
