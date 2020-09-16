---
title: Rozwiązywanie problemu — nie znaleziono użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725417"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemu — nie znaleziono użytkownika w katalogu

Jeśli użytkownicy otrzymują komunikat o błędzie "nie można odnaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu nie należy do katalogu.

Poniższe czynności można wykonać w celu rozwiązania problemu.

- Upewnij się, że konto, które zaakceptował zaproszenie pocztą e-mail, jest tego samego konta, które jest używane do logowania się później. Upewnij się, że użytkownik korzysta z tego samego konta w celu zaakceptowania zaproszenia i zarejestrowania się w witrynie. 

Aby uzyskać więcej informacji, zobacz [jak zarządzać aliasami konta Microsoft, </a> Aby zarządzać logowaniem do usługi Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Przejdź do każdej witryny, w której użytkownik otrzymuje błąd. 

Dodaj "/_layouts/15/People.aspx/MembershipGroupId = 0" (w cudzysłowach podwójnych) na koniec adresu URL witryny. 

Przykład: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wybierz użytkownika z listy.

- Kliknij pozycję **Usuń uprawnienia użytkownika** na Wstążce. 
-  Dodaj użytkownika i ponownie Wyślij zaproszenie do użytkownika.

