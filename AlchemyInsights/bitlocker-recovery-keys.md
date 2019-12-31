---
title: Klucze odzyskiwania funkcji BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908824"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="2a513-102">Uzyskiwanie dostępu do kluczy odzyskiwania funkcji BitLocker</span><span class="sxs-lookup"><span data-stu-id="2a513-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="2a513-103">Podczas konfigurowania ustawień funkcji BitLocker zasady ochrony punktu końcowego usługi Intune można określić, czy informacje odzyskiwania funkcji BitLocker mają być przechowywane w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a513-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="2a513-104">Jeśli to ustawienie jest skonfigurowane, przechowywane dane odzyskiwania powinny być widoczne dla administratora usługi Intune jako część danych rekordu urządzenia w bloku urządzenia usługi Intune na dwa sposoby:</span><span class="sxs-lookup"><span data-stu-id="2a513-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="2a513-105">Urządzenia — urządzenia z usługą Azure AD — > "urządzenie" lub urządzenia — > wszystkie urządzenia — > "urządzenie" — > klucze odzyskiwania</span><span class="sxs-lookup"><span data-stu-id="2a513-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="2a513-106">Alternatywnie, jeśli istnieje dostęp administracyjny do samego urządzenia, klucz odzyskiwania (Password) można zobaczyć, uruchamiając następujące polecenie z wiersza polecenia z podwyższonym poziomem uprawnień:</span><span class="sxs-lookup"><span data-stu-id="2a513-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="2a513-107">Jeśli urządzenie zostało zaszyfrowane przed rejestrowaniem w usłudze Intune, klucz odzyskiwania może być skojarzony z "kontem Microsoft" (MSA) używanym do logowania się do urządzenia podczas procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="2a513-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="2a513-108">Jeśli tak było, dostęp https://onedrive.live.com/recoverykey i logowanie się za pomocą tego MSA powinien pokazywać urządzenia, dla których klucze odzyskiwania były przechowywane.</span><span class="sxs-lookup"><span data-stu-id="2a513-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="2a513-109">Jeśli urządzenie zostało zaszyfrowane w wyniku konfiguracji za pomocą zasad grupy opartej na domenie, informacje o odzyskiwaniu mogą być przechowywane w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a513-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

