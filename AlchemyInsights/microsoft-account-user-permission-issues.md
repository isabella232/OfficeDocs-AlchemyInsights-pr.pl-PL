---
title: Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098180"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemów — nie można odnaleźć użytkownika w katalogu

Jeśli w katalogu jest wyświetlany komunikat o błędzie "nie można odnaleźć użytkownika" w katalogu, spróbuj ponownie, jeśli typem problemu jest Użytkownik nie w katalogu.

Aby rozwiązać ten problem, można wykonać poniższe czynności.

- Upewnij się, że konto, które zaakceptowało zaproszenie pocztą e-mail, jest tym samym kontem, które jest używane do późniejszego zalogowania się. Upewnij się, że użytkownik zaakceptuje zaproszenie i zaloguje się do witryny za pomocą tego samego konta. 

Aby uzyskać więcej informacji, zobacz [Jak zarządzać aliasami konta Microsoft </a> ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)w celu zarządzania logowaniem Microsoft 365 konta . 

- Przejdź do każdej witryny, w której użytkownik otrzymuje błąd. 

Dodaj wartość "/_layouts/15/people.aspx/membershipgroupid=0" (w cudzysłowie podwójnym) na końcu adresu URL witryny. 

Przykład: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wybierz użytkownika z listy.

- Kliknij **pozycję Usuń uprawnienia użytkowników** na Wstążce. 
-  Dodaj ponownie użytkownika i wyślij ponownie zaproszenie do użytkownika.

