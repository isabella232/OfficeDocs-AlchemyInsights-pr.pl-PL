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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768827"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="93c3a-102">Włączanie szyfrowania funkcji BitLocker za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="93c3a-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="93c3a-103">W celu skonfigurowania ustawień szyfrowania funkcji BitLocker dla urządzeń z systemem Windows można użyć zasad usługi Intune Endpoint Protection.</span><span class="sxs-lookup"><span data-stu-id="93c3a-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="93c3a-104">Aby uzyskać więcej informacji, zobacz [Ustawienia systemu Windows 10 (i nowszych wersji), aby chronić urządzenia za pomocą usługi Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="93c3a-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="93c3a-105">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji BitLocker, które zostanie wyzwolone bez zastosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="93c3a-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="93c3a-106">Może to mieć wpływ na zastosowanie zasad, jeśli są skonfigurowane ustawienia inne niż domyślne.</span><span class="sxs-lookup"><span data-stu-id="93c3a-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="93c3a-107">Aby uzyskać więcej informacji, zobacz poniższe często zadawane pytania.</span><span class="sxs-lookup"><span data-stu-id="93c3a-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="93c3a-108">Aby uzyskać informacje dotyczące rozwiązywania problemów z funkcją BitLocker, zobacz [Rozwiązywanie problemów z zasadami funkcji BitLocker w usłudze Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="93c3a-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="93c3a-109">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="93c3a-109">**FAQ**</span></span>

<span data-ttu-id="93c3a-110">P: Jakie wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad programu Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="93c3a-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="93c3a-111">O: ustawienia w zasadach programu Intune Endpoint Protection są implementowane przy użyciu [dostawcy CSP funkcji BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="93c3a-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="93c3a-112">Nie wszystkie wersje lub kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker.</span><span class="sxs-lookup"><span data-stu-id="93c3a-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="93c3a-113">P: jak można włączyć funkcję BitLocker na urządzeniach bez konieczności interakcji użytkownika końcowego?</span><span class="sxs-lookup"><span data-stu-id="93c3a-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="93c3a-114">O: tak długo, jak są spełnione wymagane wymagania wstępne, można włączyć funkcję BitLocker "ciche szyfrowanie" za pośrednictwem usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="93c3a-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="93c3a-115">Zobacz szczegółowe informacje dotyczące wymagań dotyczących urządzeń i przykładowe ustawienia zasad, aby włączyć ciche szyfrowanie w następującym dokumencie: [ciche Włączanie szyfrowania funkcji BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="93c3a-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="93c3a-116">P: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), zastosuje zasady z innymi ustawieniami automatycznie wyzwalają ponowne szyfrowanie dysku przy użyciu nowych ustawień?</span><span class="sxs-lookup"><span data-stu-id="93c3a-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="93c3a-117">O: Nie.</span><span class="sxs-lookup"><span data-stu-id="93c3a-117">A: No.</span></span> <span data-ttu-id="93c3a-118">Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.</span><span class="sxs-lookup"><span data-stu-id="93c3a-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="93c3a-119">**Uwaga:** W przypadku urządzeń, które są rejestrowane za pomocą funkcji autopilota, automatyczne szyfrowanie, które może wystąpić w trakcie OOBE, nie zostanie wyzwolone, dopóki nie zostanie wyznaczona zasada usługi Intune, co umożliwi użycie ustawień opartych na zasadach w miejsce ustawień domyślnych systemu operacyjnego.</span><span class="sxs-lookup"><span data-stu-id="93c3a-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="93c3a-120">P: Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane po usunięciu tych zasad?</span><span class="sxs-lookup"><span data-stu-id="93c3a-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="93c3a-121">A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowania skonfigurowanych dysków.</span><span class="sxs-lookup"><span data-stu-id="93c3a-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="93c3a-122">P: dlaczego zasady zgodności usługi Intune wskazują, że na moim urządzeniu nie włączono funkcji BitLocker, mimo że jest to?</span><span class="sxs-lookup"><span data-stu-id="93c3a-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="93c3a-123">A: ustawienie "włączone funkcje BitLocker" w zasadach zgodności usługi Intune korzysta z klienta usługi zaświadczeń o kondycji urządzeń systemu Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="93c3a-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="93c3a-124">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="93c3a-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="93c3a-125">Jeśli więc urządzenie nie zostało uruchomione ponownie od momentu ukończenia szyfrowania funkcją BitLocker, usługa klienta usługi DHA nie będzie raportować funkcji BitLocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="93c3a-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 