---
title: Dataprotection — funkcja BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731249"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="aa887-102">Włączanie szyfrowania funkcji BitLocker za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="aa887-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="aa887-103">W celu skonfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows można użyć zasad usługi Intune Endpoint Protection.</span><span class="sxs-lookup"><span data-stu-id="aa887-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="aa887-104">Aby uzyskać więcej informacji, zobacz [Ustawienia systemu Windows 10 (i nowszych wersji), aby chronić urządzenia za pomocą usługi Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="aa887-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="aa887-105">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji BitLocker, które zostanie wyzwolone bez zastosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="aa887-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="aa887-106">Może to mieć wpływ na zastosowanie zasad, jeśli są skonfigurowane ustawienia inne niż domyślne.</span><span class="sxs-lookup"><span data-stu-id="aa887-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="aa887-107">Aby uzyskać więcej informacji, zobacz poniższe często zadawane pytania.</span><span class="sxs-lookup"><span data-stu-id="aa887-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="aa887-108">Aby uzyskać informacje dotyczące rozwiązywania problemów z funkcją BitLocker, zobacz [Rozwiązywanie problemów z zasadami funkcji BitLocker w usłudze Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="aa887-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="aa887-109">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="aa887-109">**FAQ**</span></span>

 <span data-ttu-id="aa887-110">P: Jakie wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad programu Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="aa887-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="aa887-111">O: ustawienia w zasadach programu Intune Endpoint Protection są implementowane przy użyciu [dostawcy CSP funkcji BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="aa887-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="aa887-112">Nie wszystkie wersje lub kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker.</span><span class="sxs-lookup"><span data-stu-id="aa887-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="aa887-113">Obecnie obsługiwane są następujące wersje systemu Windows: Enterprise, Education, Mobile, Mobile Enterprise i Professional (kompilacja 1809 lub nowsza).</span><span class="sxs-lookup"><span data-stu-id="aa887-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="aa887-114">P: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), zastosuje zasady z innymi ustawieniami automatycznie wyzwalają ponowne szyfrowanie dysku przy użyciu nowych ustawień?</span><span class="sxs-lookup"><span data-stu-id="aa887-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="aa887-115">O: Nie.</span><span class="sxs-lookup"><span data-stu-id="aa887-115">A: No.</span></span> <span data-ttu-id="aa887-116">Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.</span><span class="sxs-lookup"><span data-stu-id="aa887-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="aa887-117">**Uwaga:** W przypadku urządzeń, które są rejestrowane za pomocą funkcji autopilota, automatyczne szyfrowanie, które może wystąpić w trakcie OOBE, nie zostanie wyzwolone, dopóki nie zostanie wyznaczona zasada usługi Intune, co umożliwi użycie ustawień opartych na zasadach w miejsce ustawień domyślnych systemu operacyjnego.</span><span class="sxs-lookup"><span data-stu-id="aa887-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="aa887-118">P: Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane po usunięciu tych zasad?</span><span class="sxs-lookup"><span data-stu-id="aa887-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="aa887-119">A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowania skonfigurowanych dysków.</span><span class="sxs-lookup"><span data-stu-id="aa887-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="aa887-120">P: dlaczego zasady zgodności usługi Intune wskazują, że na moim urządzeniu nie włączono funkcji BitLocker, mimo że jest to?</span><span class="sxs-lookup"><span data-stu-id="aa887-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="aa887-121">A: ustawienie "włączone funkcje BitLocker" w zasadach zgodności usługi Intune korzysta z klienta usługi zaświadczeń o kondycji urządzeń systemu Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="aa887-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="aa887-122">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="aa887-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="aa887-123">Jeśli więc urządzenie nie zostało uruchomione ponownie od momentu ukończenia szyfrowania funkcją BitLocker, usługa klienta usługi DHA nie będzie raportować funkcji BitLocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="aa887-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 