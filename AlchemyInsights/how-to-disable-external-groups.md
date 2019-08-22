---
title: Jak wyłączyć grup zewnętrznych
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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540911"
---
# <a name="how-to-disable-external-groups"></a>Jak wyłączyć grup zewnętrznych

Yammer, że obsługa wiadomości zewnętrznych stosuje reguły transportu Exchange (ETRs), zestaw proaktywne kontroli w celu zapobieżenia informacje o firmie udostępnianie. Aby ograniczyć użytkownikom możliwość tworzenia grup zewnętrznych, należy skonfigurować reguły transportu Exchange (ETR), a następnie skonfiguruj Yammer używać reguły transportu Exchange do blokowania wiadomości zewnętrznych.
  
Po utworzeniu reguły w Centrum administracyjnego programu Exchange w trybie Online, wykonaj następujące kroki, aby ustawić ETR do zastosowania w Yammer:
  
- Zaloguj się na Yammer, jako zweryfikowane i w **Centrum administracyjnego Yammer**, przejdź do C **zawartości i zabezpieczeń \> ustawienia zabezpieczeń.**

- W obszarze **Obsługa wiadomości zewnętrznych**, zaznacz **egzekwować swoje Exchange Online reguł transportu programu Exchange (ETRs) w Yammer.**

- Wybierz pozycję **Zapisz**.

Aby uzyskać więcej informacji zobacz [Kontrola zewnętrznych, obsługa wiadomości w sieci Yammer z reguły transportu Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  