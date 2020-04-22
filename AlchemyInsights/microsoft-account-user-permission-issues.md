---
title: Rozwiązywanie problemów — nie znaleziono użytkownika w katalogu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702748"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemów — nie znaleziono użytkownika w katalogu

Jeśli użytkownicy otrzymują komunikat o błędzie "nie można znaleźć użytkownika" w katalogu, spróbuj ponownie, gdzie typ problemu jest użytkownik nie w katalogu.

Poniższe kroki można wykonać, aby rozwiązać problem.

- Upewnij się, że konto, które zaakceptowało zaproszenie e-mail, jest tym samym kontem, które jest używane do późniejszego logowania. Upewnij się, że użytkownik używa tego samego konta, aby zaakceptować zaproszenie i zalogować się do witryny. 

Aby uzyskać więcej informacji, zobacz [Jak zarządzać</a> aliasami dla konta Microsoft, aby zarządzać loginem usługi Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Przejdź do każdej witryny, w której użytkownik otrzymuje błąd. 

Dodaj "/_layouts/15/people.aspx/membershipgroupid=0" (w cudzysłowach) na końcu adresu URL witryny. 

Przykład: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wybierz użytkownika z listy.

- Kliknij pozycję **Usuń uprawnienia użytkownika** ze Wstążki. 
-  Dodaj ponownie użytkownika i ponownie syłkuj zaproszenie do użytkownika.

