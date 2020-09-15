---
title: Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689964"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="33d26-102">Rozwiązywanie problemów z rejestrowaniem urządzeń z systemem Android w usłudze Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="33d26-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="33d26-103">Zapoznaj się z wymienionymi poniżej zasobami, aby rozwiązać problem teraz.</span><span class="sxs-lookup"><span data-stu-id="33d26-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="33d26-104">Oto niektóre typowe problemy i rozwiązywanie problemów:</span><span class="sxs-lookup"><span data-stu-id="33d26-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="33d26-105">**Błąd urządzenia nie zaszyfrowano w portalu firmy:** Nowsze wersje systemu Android, szczególnie w przypadku rozpoczynania pracy z wersją v 7.0, wymagają kodu dostępu, aby upewnić się, że urządzenie jest w pełni szyfrowane.</span><span class="sxs-lookup"><span data-stu-id="33d26-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="33d26-106">Typowe rozwiązania to włączenie numeru PIN uruchamiania lub pełnego zaszyfrowania urządzenia.</span><span class="sxs-lookup"><span data-stu-id="33d26-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="33d26-107">Przejrzyj [ten dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="33d26-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="33d26-108">**Urządzenia nie zapoznają się z usługą Intune ani wyświetlać jako "niezdrowe" w konsoli administracyjnej usługi Intune:** Niektóre urządzenia Samsung 4,4 i 5,5 mogą nie zaewidencjonować usługi.</span><span class="sxs-lookup"><span data-stu-id="33d26-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="33d26-109">Istnieją 3 możliwe rozwiązania tego problemu:</span><span class="sxs-lookup"><span data-stu-id="33d26-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="33d26-110">Ręcznie otwórz aplikację Portal firmy usługi Intune, co spowoduje automatyczne zainicjowanie synchronizacji urządzenia.</span><span class="sxs-lookup"><span data-stu-id="33d26-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="33d26-111">Zaktualizuj urządzenie do wersji Android 6,0 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="33d26-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="33d26-112">Wyłączenie zarządzania portalem firmowym usługi Intune przy użyciu usługi Samsung Smart Manager.</span><span class="sxs-lookup"><span data-stu-id="33d26-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="33d26-113">Przejrzyj [ten dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , aby uzyskać więcej informacji o tych problemach i rozwiązaniach.</span><span class="sxs-lookup"><span data-stu-id="33d26-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="33d26-114">**Typ licencji użytkownika jest nieprawidłowy** lub **Nazwa użytkownika nie została rozpoznana. błąd:** użytkownik musi mieć przypisaną licencję usługi Intune lub EMS.</span><span class="sxs-lookup"><span data-stu-id="33d26-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="33d26-115">Przejrzyj te dokumenty, aby przypisać licencję: Centrum administracyjne pakietu Office lub Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="33d26-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="33d26-116">Dodatkowe zasoby pomocne w rozwiązaniu problemu:</span><span class="sxs-lookup"><span data-stu-id="33d26-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="33d26-117">Skorzystaj z [portalu usługi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , aby zdiagnozować i rozwiązać typowe błędy rejestracji.</span><span class="sxs-lookup"><span data-stu-id="33d26-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="33d26-118">Przejrzyj [ten dokument](https://docs.microsoft.com/intune/help-desk-operators) , aby uzyskać więcej szczegółowych informacji.</span><span class="sxs-lookup"><span data-stu-id="33d26-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="33d26-119">Przejrzyj [ten dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , aby zapoznać się z listą typowych błędów, które uniemożliwiają rejestrowanie i rozwiązywanie problemów.</span><span class="sxs-lookup"><span data-stu-id="33d26-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="33d26-120">[Dowiedz się, jak zarejestrować urządzenia z systemem Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="33d26-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
