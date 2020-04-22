---
title: Terminy, na które brakuje w sklepie terminowym usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766863"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d6c2c-102">Włączanie szyfrowania funkcji Bitlocker za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="d6c2c-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="d6c2c-103">Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania boitlocker dla urządzeń z systemem Windows, jak opisano w : Ustawienia systemu Windows10 (i nowsze) w celu ochrony urządzeń korzystających z usługi Intune</span><span class="sxs-lookup"><span data-stu-id="d6c2c-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="d6c2c-104">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji bitlocker, które jest wyzwalane bez stosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d6c2c-105">Może to mieć wpływ na stosowanie zasad, jeśli skonfigurowano ustawienia domyślne.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="d6c2c-106">Zobacz często zadawane pytania, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-106">See FAQ for more detail.</span></span>


<span data-ttu-id="d6c2c-107">Często  zadawane pytania P: Które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?</span><span class="sxs-lookup"><span data-stu-id="d6c2c-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="d6c2c-108"> Odp.: Ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu usługi CSP funkcji Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="d6c2c-109">Nie wszystkie wersje ani kompilacje systemu Windows obsługują CSP funkcji Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="d6c2c-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="d6c2c-110">W tej chwili Windows Editions: Enterprise; Edukacja, Mobile, Mobile Enterprise i Professional (od kompilacji 1809 i 1809) są obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="d6c2c-111">Pyt.: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji Bitlocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), zastosuje zasadę z różnymi ustawieniami automatycznie wyzwala ponowne szyfrowanie dysku z nowymi ustawieniami?</span><span class="sxs-lookup"><span data-stu-id="d6c2c-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="d6c2c-112">Odp.: Nie.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-112">A: No.</span></span> <span data-ttu-id="d6c2c-113">Aby zastosować nowe ustawienia szyfrowania, dysk musi najpierw zostać odszyfrowany.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="d6c2c-114">Uwaga W przypadku urządzeń zarejestrowanych za pomocą autopilota automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostaną ocenione zasady usługi Intune, które umożliwiają użycie ustawień opartych na zasadach zamiast ustawień systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="d6c2c-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="d6c2c-115">P Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie ono odszyfrowane po usunięciu tej zasady?</span><span class="sxs-lookup"><span data-stu-id="d6c2c-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="d6c2c-116">Odp.: Usunięcie zasad związanych z szyfrowaniem NIE powoduje odszyfrowania dysków, które zostały skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="d6c2c-117">Pyt.: Dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma funkcji "Bitlocker Enabled", ale tak jest?</span><span class="sxs-lookup"><span data-stu-id="d6c2c-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="d6c2c-118">Odp.: Ustawienie "Funkcja blokowania bitów włączone" w zasadach zgodności usługi Intune wykorzystuje klienta zaświadczania kondycji urządzenia systemu Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="d6c2c-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d6c2c-119">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="d6c2c-120">Jeśli więc urządzenie nie zostało ponownie uruchomione od czasu zakończenia szyfrowania funkcji bitlocker, usługa klienta DHA nie będzie zgłaszać funkcji bitlocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="d6c2c-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>