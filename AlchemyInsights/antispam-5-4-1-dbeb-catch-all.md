---
title: AntiSpam 5.4.1 DbEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932287"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rozwiązywanie problemów dotyczących dostarczania związanych z kodem błędu 550 5.4.1 Odmowa dostępu przekazywania

Ten problem występuje podczas sprawdzania, czy adres e-mail jest prawidłowy, aby zapobiec zwrotom [zwrotnych](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) podczas wprowadzania sieci firmy Microsoft. Wypróbuj następujące czynności:

1. Określ, czy problem dotyczy całej domeny, czy pojedynczego adresu e-mail:
    - Cała domena: czasami trzeba zsynchronizować domenę. Spróbuj [zmienić domenę na Wewnętrzna, a następnie z powrotem na Autorytatywny.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Jeden adres e-mail: Czasami trzeba zsynchronizować adres; Zmiana adresu serwera proxy SMTP, a następnie jego zmiana z powrotem może pomóc.
2. Określanie, czy problem jest specyficzny dla grupy, czy folderu publicznego. W przypadku niektórych typów obiektów może być konieczne ich ręczne Azure Active Directory.

Jeśli potrzebujesz dodatkowej pomocy, otwórz bilet pomocy technicznej i określ zakres problemu (w tym typ obiektu, do który wysyłasz), abyśmy pomogli Ci pomóc.