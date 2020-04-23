---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720778"
---
# <a name="how-to-disable-external-groups"></a>Jak wyłączyć grupy zewnętrzne

Usługa Yammer wiadomości zewnętrzne stosuje Exchange Transport Rules (ETRs), zestaw proaktywnych kontroli, aby zapobiec udostępnianiu informacji o firmie. Aby ograniczyć użytkownikom możliwość tworzenia grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (ETR), a następnie skonfigurować usługę Yammer do blokowania obsługi wiadomości zewnętrznych za pomocą reguły transportu programu Exchange.
  
Po utworzeniu reguły w centrum administracyjnym usługi Exchange Online wykonaj następujące kroki, aby ustawić etr do zastosowania w usłudze Yammer:
  
- Zaloguj się do usługi Yammer jako zweryfikowany administrator, a następnie w **centrum administracyjnym usługi Yammer**przejdź do sekcji **Ustawienia zawartości i zabezpieczeń C. \> **

- W obszarze **Wiadomości zewnętrzne**wybierz pozycję **Wymuszaj reguły transportu wymiany online (ETR) w usłudze Yammer.**

- Wybierz pozycję **Zapisz**.

Aby uzyskać więcej informacji, zobacz [Wyłączanie wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  