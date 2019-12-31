---
title: DataProtection — funkcja BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908719"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="6f3a8-102">Włączanie szyfrowania funkcją BitLocker w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="6f3a8-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="6f3a8-103">Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="6f3a8-104">Aby uzyskać więcej informacji, zobacz [Ustawienia systemu Windows 10 (i nowsze), aby chronić urządzenia przy użyciu usługi Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="6f3a8-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="6f3a8-105">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcją BitLocker, który jest wyzwalany bez stosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="6f3a8-106">Może to wpłynąć na stosowanie zasad, jeśli skonfigurowano inne niż domyślne ustawienia.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="6f3a8-107">Zobacz następujące FAQ, aby uzyskać więcej szczegółów.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="6f3a8-108">Aby uzyskać informacje dotyczące rozwiązywania problemów z funkcją BitLocker, zobacz Rozwiązywanie problemów z [zasadami funkcji BitLocker w usłudze Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="6f3a8-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="6f3a8-109">**Często zadawane pytania**</span><span class="sxs-lookup"><span data-stu-id="6f3a8-109">**FAQ**</span></span>

 <span data-ttu-id="6f3a8-110">P: które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?</span><span class="sxs-lookup"><span data-stu-id="6f3a8-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="6f3a8-111">A: ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu [dostawcy CSP funkcji BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="6f3a8-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="6f3a8-112">Nie wszystkie edycje lub kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="6f3a8-113">W tej chwili obsługiwane są następujące wersje systemu Windows: Enterprise, edukacja, komórka, Mobile Enterprise i Professional (kompilacja 1809 i nowsze).</span><span class="sxs-lookup"><span data-stu-id="6f3a8-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="6f3a8-114">Q: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfru (XTS-AES-128), będzie stosowanie zasad z różnych ustawień automatycznie wyzwolić ponowne szyfrowanie dysku z nowymi ustawieniami?</span><span class="sxs-lookup"><span data-stu-id="6f3a8-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="6f3a8-115">O: nie.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-115">A: No.</span></span> <span data-ttu-id="6f3a8-116">Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="6f3a8-117">**Uwaga:** W przypadku urządzeń zarejestrowanych w programie autopilot automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostanie oszacowana zasada usługi Intune, co umożliwi ustawienia oparte na zasadach, które będą używane zamiast ustawień domyślnych systemu operacyjnego.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="6f3a8-118">P: Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie ono odszyfrowane po usunięciu tej zasady?</span><span class="sxs-lookup"><span data-stu-id="6f3a8-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="6f3a8-119">A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowywania dysków, które zostały skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="6f3a8-120">Q: dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma włączoną funkcją BitLocker, mimo że jest?</span><span class="sxs-lookup"><span data-stu-id="6f3a8-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="6f3a8-121">A: ustawienie "włączona funkcja BitLocker" w zasadach zgodności usługi Intune korzysta z klienta Windows Device atestacja zdrowia (DHA).</span><span class="sxs-lookup"><span data-stu-id="6f3a8-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="6f3a8-122">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="6f3a8-123">Jeśli więc urządzenie nie zostało ponownie uruchomiony od czasu ukończenia szyfrowania funkcją BitLocker, usługa klienta DHA nie będzie raportować funkcji BitLocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="6f3a8-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 