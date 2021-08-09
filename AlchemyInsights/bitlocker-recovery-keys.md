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
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060074"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Uzyskiwanie dostępu do kluczy odzyskiwania funkcji BitLocker

Podczas konfigurowania ustawień funkcji BitLocker Intune Endpoint Protection usługi Intune można określić, czy informacje o odzyskiwaniu funkcji BitLocker mają być przechowywane w usłudze Azure Active Directory.

Jeśli to ustawienie jest skonfigurowane, przechowywane dane odzyskiwania powinny być widoczne dla administratora usługi Intune jako część danych rekordu urządzenia w urządzeniu blade w usłudze Intune Na dwa sposoby:

Urządzenia — urządzenia usługi Azure AD > "Urządzenie" LUB Urządzenia > Wszystkie urządzenia > "Urządzenie" -> Klucze odzyskiwania

Ewentualnie, jeśli istnieje administracyjny dostęp do samego urządzenia, klucz odzyskiwania (Hasło) jest widoczny, uruchamiając następujące polecenie z poziomu wiersza polecenia z podwyższonym poziomem uprawnień:

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
Jeśli urządzenie zostało zaszyfrowane przed rozpoczęciem korzystania z usługi Intune, klucz odzyskiwania mógł zostać skojarzony z kontem Microsoft (MSA) używanym do logowania się na urządzeniu podczas procesu OOBE. W takim przypadku uzyskiwanie dostępu do tego konta MSA i logowanie się za jego pomocą powinno pokazywać urządzenia, na których były  https://onedrive.live.com/recoverykey przechowywane klucze odzyskiwania.
 
Jeśli urządzenie zostało zaszyfrowane w wyniku konfiguracji za pośrednictwem zasad grupy opartych na domenie, informacje o odzyskiwaniu mogą być przechowywane w lokalnej usłudze Active Directory.

Jeśli skonfigurowano zasady ochrony punktu końcowego do przechowywania klucza odzyskiwania w programie Azure Active Directory ale klucz określonego urządzenia nie został przekazany, możesz wyzwolić przekazywanie, obracając klucz odzyskiwania dla tego urządzenia z konsoli MEM. Aby uzyskać szczegółowe informacje, [zobacz Obracanie kluczy odzyskiwania funkcji BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

