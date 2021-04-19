---
title: Adresowanie błędu logowania do zespołów AADSTS9000411
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
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821997"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresowanie błędu logowania do zespołów AADSTS9000411

Podczas logowania się do aplikacji Microsoft Teams może zostać wyświetlony komunikat o błędzie: Niestety, ale mamy problem z zalogowaniem Cię do **AADSTS9000411: Żądanie nie jest poprawnie sformatowane. Parametr "login_hint" został zduplikowany.**

Aby rozwiązać ten problem, upewnij się, że Twoi klienci aplikacji Microsoft Teams są zaktualizowani. Aby uzyskać więcej informacji na temat aktualizowania klienta, zobacz [Aktualizowanie aplikacji Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Jeśli z jakiegoś powodu nie możesz zaktualizować klienta, wylogowanie się z klienta spowoduje wyczyszczenie większości danych buforowanych. Jeśli jednak po zalogowaniu/zalogowaniu nadal masz problemy, zamknij usługę Teams i wyczyść pamięć podręczną klienta, wykonując następujące czynności:
1. Zamknij usługę Microsoft Teams.
2. Przejdź do: %appdata%\microsoft\teams i usuń wszystkie pliki.
3. Otwórz ponownie usługę Microsoft Teams.
