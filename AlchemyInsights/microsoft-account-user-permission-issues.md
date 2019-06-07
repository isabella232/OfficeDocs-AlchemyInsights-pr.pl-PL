---
title: Tworzenie i używanie udostępnionej skrzynki pocztowej
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762410"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rozwiązywanie problemu - nie można odnaleźć w katalogu użytkownika

Jeśli użytkownicy otrzymują błąd komunikat "nie można znaleźć użytkownika" w katalogu. Spróbuj ponownie gdzie typ problemu użytkownika nie jest w katalogu.

Następujące czynności mogą być wykonywane w celu rozwiązania problemu.

- Upewnij się, konto, na którym przyjęte wiadomości e-mail z zaproszeniem jest to samo konto, który jest używany do logowania się później. Upewnij się, że użytkownik korzysta z tego samego konta aby zaakceptować zaproszenie i zalogować się do witryny. 

Aby uzyskać więcej informacji, zobacz [sposobu zarządzania aliasy konta Microsoft</a> do zarządzania logowania usługi Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Przejdź do każdej witryny, w której użytkownik odbiera błąd. 

Dodać "/ _layouts/15/people.aspx/membershipgroupid=0" (ujęty w cudzysłów podwójny) na końcu adresu URL witryny. 

Przykład: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wybierz użytkownika z listy.

- Kliknij przycisk **Usuń uprawnienia użytkownika** na Wstążce. 
-  Dodać z powrotem użytkownika i ponownie wysłać zaproszenia do użytkownika.

