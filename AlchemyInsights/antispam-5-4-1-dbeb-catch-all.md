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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707921"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rozwiązywanie problemów z dostarczaniem kodu błędu 550 5.4.1 Odmowa dostępu do przekaźnika

Ten problem występuje podczas [sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec odbijaniu podczas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) wchodzenia do sieci firmy Microsoft. Spróbuj wykonać następujące czynności:

1. Określ, czy problem dotyczy całej domeny, czy pojedynczego adresu e-mail:
    - Cała domena: czasami domena musi być zsynchronizowana; spróbuj [skonfigurować domenę na Wewnętrzną, a następnie wróć do Autorytatywny](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Pojedynczy adres e-mail: czasami adres musi być zsynchronizowany; zmiana adresu proxy smtp, a następnie zmiana go z powrotem może pomóc.
2. Określ, czy problem jest specyficzny dla grupy lub folderu publicznego. W przypadku niektórych typów obiektów obiekty mogą wymagać ręcznego utworzenia w usłudze Azure Active Directory.

Jeśli potrzebujesz dodatkowej pomocy, otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do którego wysyłasz), abyśmy mogli ci lepiej pomóc.