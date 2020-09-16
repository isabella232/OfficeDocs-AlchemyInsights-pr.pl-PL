---
title: Brakuje terminów w magazynie terminów usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750461"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ea8be-102">Włączanie szyfrowania funkcji BitLocker za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="ea8be-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="ea8be-103">Zasady usługi Intune Endpoint Protection mogą być używane do konfigurowania ustawień szyfrowania Boitlocker dla urządzeń z systemem Windows, zgodnie z opisem w następujących systemach: Windows10 (i nowszych) w celu ochrony urządzeń przy użyciu usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="ea8be-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="ea8be-104">Należy pamiętać, że wiele nowszych urządzeń z systemem Windows 10 obsługuje automatyczne szyfrowanie funkcji BitLocker, które zostanie wyzwolone bez zastosowania zasad MDM.</span><span class="sxs-lookup"><span data-stu-id="ea8be-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ea8be-105">Może to mieć wpływ na zastosowanie zasad, jeśli nie skonfigurowano ustawień niedomyślnych.</span><span class="sxs-lookup"><span data-stu-id="ea8be-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="ea8be-106">Zobacz często zadawane pytania, aby uzyskać więcej szczegółowych informacji.</span><span class="sxs-lookup"><span data-stu-id="ea8be-106">See FAQ for more detail.</span></span>


<span data-ttu-id="ea8be-107">Często zadawane pytania   p: Jakie wersje systemu Windows obsługują szyfrowanie urządzeń przy użyciu zasad programu Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="ea8be-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="ea8be-108"> O: ustawienia w zasadach programu Intune Endpoint Protection są implementowane przy użyciu dostawcy CSP funkcji BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ea8be-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="ea8be-109">Nie wszystkie wersje i kompilacje systemu Windows obsługują dostawcę CSP funkcji BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="ea8be-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="ea8be-110">W tym momencie wersja systemu Windows: Enterprise; Obsługiwane są wykształcenie, telefony komórkowe, telefony komórkowe i profesjonalne (od kompilacji 1809).</span><span class="sxs-lookup"><span data-stu-id="ea8be-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="ea8be-111">P: Jeśli urządzenie jest już zaszyfrowane za pomocą funkcji BitLocker przy użyciu domyślnych ustawień systemu operacyjnego dla metody szyfrowania i siły szyfrowania (XTS-AES-128), będą stosowane zasady z różnymi ustawieniami automatycznie wyzwalać ponowne szyfrowanie dysku przy użyciu nowych ustawień?</span><span class="sxs-lookup"><span data-stu-id="ea8be-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="ea8be-112">O: Nie.</span><span class="sxs-lookup"><span data-stu-id="ea8be-112">A: No.</span></span> <span data-ttu-id="ea8be-113">Aby zastosować nowe ustawienia szyfru, należy najpierw odszyfrować dysk.</span><span class="sxs-lookup"><span data-stu-id="ea8be-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="ea8be-114">Uwaga dotycząca urządzeń zarejestrowanych za pomocą autopilota automatyczne szyfrowanie, które może wystąpić w trakcie OOBE, nie zostanie wyzwolone, dopóki nie zostanie wykryta zasada usługi Intune, która zezwala na użycie ustawień opartych na zasadach w miejscu domyślnym systemu operacyjnego</span><span class="sxs-lookup"><span data-stu-id="ea8be-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="ea8be-115">P Jeśli urządzenie jest szyfrowane w wyniku zastosowania zasad usługi Intune, zostanie odszyfrowane po usunięciu tych zasad?</span><span class="sxs-lookup"><span data-stu-id="ea8be-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="ea8be-116">A: usunięcie zasad związanych z szyfrowaniem nie powoduje odszyfrowania dysków, które zostały skonfigurowane.</span><span class="sxs-lookup"><span data-stu-id="ea8be-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="ea8be-117">P: dlaczego zasady zgodności usługi Intune wskazują, że na moim urządzeniu nie włączono funkcji "BitLocker Enabled", ale jest to?</span><span class="sxs-lookup"><span data-stu-id="ea8be-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="ea8be-118">A: ustawienie "włączone funkcje BitLocker" w zasadach zgodności usługi Intune korzysta z klienta usługi zaświadczeń o kondycji urządzeń systemu Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="ea8be-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ea8be-119">Ten klient mierzy tylko stan urządzenia w czasie rozruchu.</span><span class="sxs-lookup"><span data-stu-id="ea8be-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="ea8be-120">Jeśli więc urządzenie nie zostało uruchomione ponownie od momentu ukończenia szyfrowania funkcją BitLocker, usługa klienta DHA nie będzie raportować funkcji BitLocker jako aktywnej.</span><span class="sxs-lookup"><span data-stu-id="ea8be-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>