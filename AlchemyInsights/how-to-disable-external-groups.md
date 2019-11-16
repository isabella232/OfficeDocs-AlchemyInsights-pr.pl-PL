---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739503"
---
# <a name="how-to-disable-external-groups"></a>Jak wyłączyć grupy zewnętrzne

Yammer wiadomości zewnętrznych stosuje zasady transportu Exchange (ETRs), zestaw aktywnych formantów, aby zapobiec udostępnianiu informacji o firmie. Aby ograniczyć użytkownikom tworzenie grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (ETR), a następnie skonfigurować Yammer do używania reguły transportu programu Exchange do blokowania wiadomości zewnętrznych.
  
Po utworzeniu reguły w centrum administracyjnym programu Exchange Online, wykonaj następujące kroki, aby ustawić ETR do zastosowania w Yammer:
  
- Zaloguj się do Yammer jako zweryfikowanego administratora, a w **centrum administracyjnym Yammer**przejdź do **zawartości C i ustawienia \> zabezpieczeń zabezpieczeń.**

- W obszarze **wiadomości zewnętrznych**, wybierz opcję **Wymuszaj Exchange Online Exchange Transport Rules (ETRs) w Yammer.**

- Wybierz pozycję **Zapisz**.

Aby uzyskać więcej informacji, zobacz [wyłączanie obsługi wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  