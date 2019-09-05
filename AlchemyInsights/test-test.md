---
title: Terminy brakujące w usłudze SharePoint Online Term Store
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762079"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5e7f1-102">Włączanie szyfrowania funkcją BitLocker w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="5e7f1-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5e7f1-103">Zasady ochrony punktu końcowego usługi Intune mogą służyć do konfigurowania ustawień szyfrowania Boitlocker dla urządzeń z systemem Windows zgodnie z opisem w: ustawienia Windows10 (i nowsze) w celu ochrony urządzeń przy użyciu usługi Intune</span><span class="sxs-lookup"><span data-stu-id="5e7f1-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5e7f1-104">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcją BitLocker, który jest wyzwalany bez stosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5e7f1-105">Może to wpłynąć na stosowanie zasad, jeśli nie skonfigurowano ustawień domyślnych.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5e7f1-106">Więcej szczegółów znajdziesz w FAQ.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5e7f1-107">Często  zadawane pytania Q: które wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad ochrony punktu końcowego?</span><span class="sxs-lookup"><span data-stu-id="5e7f1-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5e7f1-108"> A: ustawienia w zasadach ochrony punktu końcowego usługi Intune są implementowane przy użyciu programu CSP funkcji BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5e7f1-109">Nie wszystkie edycje ani kompilacje systemu Windows nie obsługują programu CSP funkcji BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="5e7f1-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5e7f1-110">W tej chwili wersje systemu Windows: Enterprise; Edukacja, komórka, Mobile Enterprise i Professional (od Build 1809 i nowsze) są obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5e7f1-111">Q: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfru (XTS-AES-128) będzie stosowanie zasad z różnych ustawień automatycznie wyzwolić ponowne szyfrowanie dysku z nowymi ustawieniami?</span><span class="sxs-lookup"><span data-stu-id="5e7f1-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5e7f1-112">O: nie.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-112">A: No.</span></span> <span data-ttu-id="5e7f1-113">Aby zastosować nowe ustawienia szyfrowania, należy najpierw odszyfrować dysk.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5e7f1-114">Uwaga w przypadku urządzeń zarejestrowanych w programie autopilot automatyczne szyfrowanie, które miałoby miejsce podczas OOBE, nie jest wyzwalane, dopóki nie zostanie oszacowana zasada usługi Intune, która zezwala na korzystanie z ustawień opartych na zasadach zamiast wartości domyślnych systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="5e7f1-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5e7f1-115">Q Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune zostanie on odszyfrowany po usunięciu tej zasady?</span><span class="sxs-lookup"><span data-stu-id="5e7f1-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5e7f1-116">A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowywania dysków, które zostały skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5e7f1-117">P: dlaczego zasady zgodności usługi Intune pokazują, że moje urządzenie nie ma "włączoną funkcją BitLocker", ale jest?</span><span class="sxs-lookup"><span data-stu-id="5e7f1-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5e7f1-118">A: ustawienie "włączona funkcja BitLocker" w zasadach zgodności usługi Intune korzysta z klienta Windows Device Health atestacja (DHA).</span><span class="sxs-lookup"><span data-stu-id="5e7f1-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5e7f1-119">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5e7f1-120">Jeśli więc urządzenie nie zostało ponownie uruchomiony, ponieważ szyfrowanie funkcją BitLocker zostało zakończone, usługa klienta DHA nie zgłosi funkcji BitLocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>