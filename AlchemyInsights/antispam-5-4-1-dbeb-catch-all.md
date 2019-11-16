---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672443"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rozwiązywanie problemów z dostarczaniem kodu błędu 550 5.4.1 odmowa dostępu do przekaźnika

Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wprowadzania sieci 365 pakietu Office. Wypróbuj następujące:

1. Określ, czy problem dotyczy całej domeny, czy jednego adresu e-mail:
    - Cała domena: czasami domena musi być synchronizowana; Spróbuj [ustawić domenę jako wewnętrzną, a następnie wróć do autorytatywnych](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Pojedynczy adres e-mail: Czasami adres musi być zsynchronizowany; zmienić adres serwera proxy SMTP, a następnie zmienić go z powrotem może pomóc.
2. Określić, czy problem jest specyficzny dla grupy lub folderu publicznego. W przypadku niektórych typów obiektów może być konieczne ręczne utworzenie w usłudze Azure Active Directory.

Jeśli potrzebujesz dodatkowej pomocy, Otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do którego wysyłasz), abyśmy mogli pomóc Ci lepiej.