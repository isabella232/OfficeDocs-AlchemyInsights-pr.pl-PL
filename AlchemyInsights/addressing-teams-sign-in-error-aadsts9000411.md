---
title: Błąd logowania zespołów adresowania AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357874"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Błąd logowania zespołów adresowania AADSTS9000411

Podczas logowania się do usługi Microsoft Teams może pojawić się błąd: **Przepraszamy, ale mamy problemy z podpisywaniem Cię w Usłudze AADSTS9000411: Żądanie nie jest poprawnie sformatowane. Parametr "login_hint" jest duplikowany.**

Aby rozwiązać ten problem, upewnij się, że klienci usługi Microsoft Teams są aktualizowani. Aby uzyskać więcej informacji na temat aktualizowania klienta, zobacz [Aktualizowanie usługi Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Jeśli nie można zaktualizować klienta z jakiegoś powodu, wylogowanie klienta spowoduje wyczyszczenie większości danych w pamięci podręcznej. Jeśli jednak nadal występują problemy po wylogowaniu/logowaniu, zamknij program Teams i wyczyść pamięć podręczną klienta, wykonując następujące czynności:
1. Zamknij usługi Microsoft Teams.
2. Przejdź do: %appdata%\microsoft\teams i usuń wszystkie pliki.
3. Ponowne otwarcie usługi Microsoft Teams.
