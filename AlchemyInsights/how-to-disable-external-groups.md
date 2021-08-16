---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015630"
---
# <a name="how-to-disable-external-groups"></a>Jak wyłączyć grupy zewnętrzne

Yammer wiadomości zewnętrzne Exchange reguły transportu (ET) to zestaw proaktywnych działań, które zapobiegają udostępnianiu informacji firmowych. Aby uniemożliwić użytkownikom tworzenie grup zewnętrznych, musisz skonfigurować regułę transportu Exchange (ETR), a następnie skonfigurować usługę Yammer w celu blokowania wiadomości zewnętrznych za pomocą reguły transportu Exchange.
  
Po utworzeniu reguły w centrum administracyjnym usługi Exchange Online wykonaj następujące czynności, aby ustawić stosowanie reguły w programie Yammer:
  
- Zaloguj się Yammer jako zweryfikowany administrator, a następnie w centrum administracyjnym usługi **Yammer** przejdź do pozycji Zawartość i zabezpieczenia C w centrum **\> Ustawienia.**

- W **obszarze Wiadomości zewnętrzne** wybierz pozycję **Wymusz reguły transportu Exchange Online Exchange (EPR) w Yammer.**

- Wybierz pozycję **Zapisz**.

Aby uzyskać więcej informacji, [zobacz Wyłączanie wiadomości zewnętrznych w Yammer sieci.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  