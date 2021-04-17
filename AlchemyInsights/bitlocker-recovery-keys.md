---
title: Klucze odzyskiwania funkcji BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820296"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="61c0f-102">Uzyskiwanie dostępu do kluczy odzyskiwania funkcji BitLocker</span><span class="sxs-lookup"><span data-stu-id="61c0f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="61c0f-103">Podczas konfigurowania ustawień funkcji BitLocker Zasady ochrony punktu końcowego usługi Intune można określić, czy informacje o odzyskiwaniu funkcji BitLocker mają być przechowywane w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61c0f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="61c0f-104">Jeśli to ustawienie jest skonfigurowane, przechowywane dane odzyskiwania powinny być widoczne dla administratora usługi Intune jako część danych rekordu urządzenia w urządzeniu blade w usłudze Intune Na dwa sposoby:</span><span class="sxs-lookup"><span data-stu-id="61c0f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="61c0f-105">Urządzenia — urządzenia usługi Azure AD > "Urządzenie" LUB Urządzenia > Wszystkie urządzenia > "Urządzenie" -> Klucze odzyskiwania</span><span class="sxs-lookup"><span data-stu-id="61c0f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="61c0f-106">Ewentualnie, jeśli istnieje administracyjny dostęp do samego urządzenia, klucz odzyskiwania (Hasło) jest widoczny, uruchamiając następujące polecenie z poziomu wiersza polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="61c0f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="61c0f-107">Jeśli urządzenie zostało zaszyfrowane przed rozpoczęciem korzystania z usługi Intune, klucz odzyskiwania mógł zostać skojarzony z kontem Microsoft (MSA) używanym do logowania się na urządzeniu podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="61c0f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="61c0f-108">W takim przypadku uzyskiwanie dostępu do tego konta MSA i logowanie się za jego pomocą powinno pokazywać urządzenia, na których były  https://onedrive.live.com/recoverykey przechowywane klucze odzyskiwania.</span><span class="sxs-lookup"><span data-stu-id="61c0f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="61c0f-109">Jeśli urządzenie zostało zaszyfrowane w wyniku konfiguracji za pośrednictwem zasad grupy opartych na domenie, informacje o odzyskiwaniu mogą być przechowywane w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61c0f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="61c0f-110">Jeśli skonfigurowano zasady ochrony punktu końcowego do przechowywania klucza odzyskiwania w usłudze Azure Active Directory, ale klucz określonego urządzenia nie został przekazany, możesz wyzwolić przekazywanie, obracając klucz odzyskiwania dla tego urządzenia z konsoli MEM.</span><span class="sxs-lookup"><span data-stu-id="61c0f-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="61c0f-111">Aby uzyskać szczegółowe informacje, [zobacz Obracanie kluczy odzyskiwania funkcji BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="61c0f-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

