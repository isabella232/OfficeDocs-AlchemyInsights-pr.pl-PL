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
# <a name="accessing-bitlocker-recovery-keys"></a>Uzyskiwanie dostępu do kluczy odzyskiwania funkcji BitLocker

Podczas konfigurowania ustawień funkcji BitLocker zasady ochrony punktu końcowego usługi Intune można określić, czy informacje odzyskiwania funkcji BitLocker mają być przechowywane w usłudze Azure Active Directory.

Jeśli to ustawienie jest skonfigurowane, przechowywane dane odzyskiwania powinny być widoczne dla administratora usługi Intune jako część danych rekordu urządzenia w bloku urządzenia usługi Intune na dwa sposoby:

Urządzenia — urządzenia z usługą Azure AD — > "urządzenie" lub urządzenia — > wszystkie urządzenia — > "urządzenie" — > klucze odzyskiwania

Alternatywnie, jeśli istnieje dostęp administracyjny do samego urządzenia, klucz odzyskiwania (Password) można zobaczyć, uruchamiając następujące polecenie z wiersza polecenia z podwyższonym poziomem uprawnień:

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
Jeśli urządzenie zostało zaszyfrowane przed rejestrowaniem w usłudze Intune, klucz odzyskiwania może być skojarzony z "kontem Microsoft" (MSA) używanym do logowania się do urządzenia podczas procesu OOBE. Jeśli tak było, dostęp https://onedrive.live.com/recoverykey i logowanie się za pomocą tego MSA powinien pokazywać urządzenia, dla których klucze odzyskiwania były przechowywane.
 
Jeśli urządzenie zostało zaszyfrowane w wyniku konfiguracji za pomocą zasad grupy opartej na domenie, informacje o odzyskiwaniu mogą być przechowywane w lokalnej usłudze Active Directory.
 

