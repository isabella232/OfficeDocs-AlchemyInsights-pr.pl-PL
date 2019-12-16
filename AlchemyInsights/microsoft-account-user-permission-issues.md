---
title: Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054820"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu

Jeśli użytkownicy otrzymują komunikat o błędzie "nie można znaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu jest użytkownik nie w katalogu.

Aby rozwiązać ten problem, można wykonać następujące czynności.

- Upewnij się, że konto, które zaakceptował zaproszenie e-mail jest to samo konto, które jest używane do logowania się później. Upewnij się, że użytkownik korzysta z tego samego konta, aby zaakceptować zaproszenie i zalogować się do witryny. 

Aby uzyskać więcej informacji, zobacz [jak zarządzać aliasami konta</a> Microsoft w celu zarządzania biurem 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Przejdź do każdej witryny, w którym użytkownik otrzymuje błąd. 

Dodaj "/_layouts/15/People.aspx/MembershipGroupId = 0" (w cudzysłowie) na końcu adresu URL witryny. 

Przykład: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wybierz użytkownika z listy.

- Kliknij przycisk **Usuń uprawnienia użytkownika** ze wstążki. 
-  Dodaj ponownie użytkownika i ponownie Wyślij zaproszenie do użytkownika.

