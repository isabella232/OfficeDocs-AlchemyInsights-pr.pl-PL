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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704138"
---
# <a name="how-to-disable-external-groups"></a>Jak wyłączyć grupy zewnętrzne

Komunikacja zewnętrzna usługi Yammer umożliwia stosowanie reguł transportu programu Exchange (ETR), zestawu aktywnych kontrolek w celu uniemożliwienia udostępniania informacji o firmie. Aby uniemożliwić użytkownikom tworzenie grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (regułę), a następnie skonfigurować usługę Yammer do korzystania z reguły transportu programu Exchange w celu blokowania wiadomości zewnętrznych.
  
Po utworzeniu reguły w centrum administracyjnym usługi Exchange Online wykonaj poniższe czynności, aby ustawić regułę do zastosowania w usłudze Yammer:
  
- Zaloguj się do usługi Yammer jako zweryfikowany administrator, a następnie w **centrum administracyjnym usługi Yammer**przejdź do obszaru C ** \> Ustawienia zabezpieczeń zawartości i zabezpieczeń.**

- W obszarze **wiadomości zewnętrzne**wybierz pozycję **Wymuś reguły transportu usługi Exchange Online Exchange (ETR) w usłudze Yammer.**

- Wybierz pozycję **Zapisz**.

Aby uzyskać więcej informacji, zobacz [wyłączanie wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  