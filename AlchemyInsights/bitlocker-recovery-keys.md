---
title: Klucze odzyskiwania funkcji BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685896"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Uzyskiwanie dostępu do kluczy odzyskiwania funkcji BitLocker

Konfigurując ustawienia funkcji BitLocker w usłudze Intune Endpoint Protection, można określić, czy informacje odzyskiwania funkcji BitLocker mają być przechowywane w usłudze Azure Active Directory.

Jeśli to ustawienie zostanie skonfigurowane, dane odzyskiwania będą widoczne dla administratora usługi Intune jako część danych rekordu urządzenia w bloku urządzenia usługi Intune na dwa sposoby:

Urządzenia — urządzenia usługi Azure AD — > "urządzenie" lub urządzenia — > wszystkich urządzeń-> kluczy odzyskiwania "urządzenie"->

Jeśli masz dostęp administracyjny do samego urządzenia, możesz wyświetlić klucz odzyskiwania (hasło), uruchamiając następujące polecenie w wierszu polecenia z podwyższonym poziomem uprawnień:

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
Jeśli urządzenie zostało zaszyfrowane przed rozpoczęciem rejestracji w usłudze Intune, klucz odzyskiwania może być skojarzony z "kontem Microsoft" (MSA) używanym do logowania się do urządzenia w trakcie procesu OOBE. W takim przypadku dostęp  https://onedrive.live.com/recoverykey i logowanie się przy użyciu tego konta MSA powinno pokazywać urządzenia, dla których są przechowywane klucze odzyskiwania.
 
Jeśli urządzenie zostało zaszyfrowane w wyniku konfiguracji za pośrednictwem zasad grupy opartych na domenie, informacje odzyskiwania mogą być przechowywane w lokalnej usłudze Active Directory.
 

