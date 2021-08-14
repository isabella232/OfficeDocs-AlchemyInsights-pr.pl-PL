---
title: Adresowanie Teams błędu logowania AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953045"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresowanie Teams błędu logowania AADSTS9000411

Podczas logowania się do Microsoft Teams może zostać wyświetlony komunikat o błędzie: Niestety, ale mamy problem z zalogowaniem Cię w aplikacji **AADSTS9000411: Żądanie nie jest poprawnie sformatowane. Parametr "login_hint" został zduplikowany.**

Aby rozwiązać ten problem, upewnij się, że Microsoft Teams klienci są zaktualizowani. Aby uzyskać więcej informacji na temat aktualizowania klienta, [zobacz Aktualizowanie Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Jeśli z jakiegoś powodu nie możesz zaktualizować klienta, wylogowanie się z klienta spowoduje wyczyszczenie większości danych buforowanych. Jeśli jednak po zalogowaniu/zalogowaniu nadal masz problemy, zamknij program Teams i wyczyść pamięć podręczną klienta, wykonując następujące czynności:
1. Zamknij Microsoft Teams.
2. Przejdź do: %appdata%\microsoft\teams i usuń wszystkie pliki.
3. Otwórz ponownie Microsoft Teams.
