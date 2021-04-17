---
title: Utwórz wiadomość e-mail, aby wszystkie
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816210"
---
# <a name="create-an-email-catch-all"></a>Utwórz wiadomość e-mail, aby wszystkie

Korzystanie z tego wszystkiego jest stanowczo zalecane. Lepiej wrócić do nadawcy, aby nadawca wiedział, że jego wiadomość nie może zostać dostarczona jako zaadresowana, aby mogli podjąć działania. Monitorowaną skrzynkę pocztową można również ograniczyć do tylko tych, które wcześniej były prawidłowe. 

Każdy chwyć całą skrzynkę pocztową otrzyma dużo spamu i może zostać w końcu zapełnienie, jeśli nie będzie ściśle monitorowane. (Istnieją limity). 

Jeśli zdecydujesz się kontynuować, wykonaj następujące czynności:

1. Utwórz dynamiczną grupę dystrybucyjną, & dołącz "Wszystkie typy adresatów".

2. Utwórz dedykowaną skrzynkę pocztową, aby chwyć wiadomości e-mail, na catchall@domain.com.

3. Dla określonej domeny ustaw dla ustawienia DomainType wartość "InternalRelay". Jeśli później usuniesz wszystkie ustawienia, upewnij się, że domena ma ustawioną wartość Autorytatywny.

4. Utwórz regułę transportu przepływu poczty e-mail w następujący sposób:

    - Jeśli nadawca to "Spoza organizacji"
    - Przekieruj wiadomość do Catchall@domain.com
    - Za wyjątkiem, jeśli adresat jest członkiem grupy allusers@domain.com (grupa dystrybucyjna zawiera wszystkich członków)
    - Sprawdzanie, czy nowe skrzynki pocztowe zostały dodane do dynamicznej grupy dystrybucyjnej
