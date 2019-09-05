---
title: Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754202"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu

Jeśli użytkownicy otrzymują komunikat o błędzie "nie można odnaleźć użytkownika" w katalogu. Proszę spróbować ponownie gdzie typ problemu jest użytkownik nie w katalogu.

Aby rozwiązać ten problem, można wykonać następujące czynności.

- Upewnij się, że konto, które zaakceptował zaproszenie e-mail jest to samo konto, które jest używane do logowania się później. Upewnij się, że użytkownik korzysta z tego samego konta, aby zaakceptować zaproszenie i zalogować się do witryny. 

Aby uzyskać więcej informacji, zobacz [jak zarządzać aliasami konta</a> Microsoft w celu zarządzania biurem 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Przejdź do każdej witryny, w którym użytkownik otrzymuje błąd. 

Dodaj "/_layouts/15/People.aspx/MembershipGroupId = 0" (w cudzysłowie) na końcu adresu URL witryny. 

Przykład: https://_LT_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.

- Wybierz użytkownika z listy.

- Kliknij przycisk **Usuń uprawnienia użytkownika** ze wstążki. 
-  Dodaj ponownie użytkownika i ponownie Wyślij zaproszenie do użytkownika.

