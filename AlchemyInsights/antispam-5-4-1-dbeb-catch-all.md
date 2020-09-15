---
title: AntiSpam 5.4.1 DBEB-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717371"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rozwiązywanie problemów dotyczących dostarczania kodu błędu 550 5.4.1 Przekazywanie dostępu

Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wchodzenia do sieci Microsoft Network. Spróbuj wykonać następujące czynności:

1. Ustal, czy problem dotyczy całej domeny, czy jednego adresu e-mail:
    - Cała domena: Czasami trzeba zsynchronizować domenę; Spróbuj [skonfigurować domenę jako wewnętrzną, a następnie ponownie na autorytatywną](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jeden adres e-mail: Czasami należy zsynchronizować adres; Zmiana adresu serwera proxy SMTP, a następnie jego ponownej zmiany może pomóc.
2. Ustal, czy problem dotyczy grupy, czy folderu publicznego. W przypadku niektórych typów obiektów w usłudze Azure Active Directory może być konieczne ręczne utworzenie obiektu.

Jeśli potrzebujesz dodatkowej pomocy, Otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, na który wysyłasz), dzięki czemu możemy pomóc Ci lepiej.