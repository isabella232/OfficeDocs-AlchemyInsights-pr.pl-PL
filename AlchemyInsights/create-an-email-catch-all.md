---
title: Tworzenie wiadomości e-mail z całą połową
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712996"
---
# <a name="create-an-email-catch-all"></a>Tworzenie wiadomości e-mail z całą połową

Korzystanie z funkcji catch all nie jest zalecane. Lepszym rozwiązaniem jest dostarczenie odskakującego przeskoku nadawcy informującego, że nadawcy nie będą wiedzieli, że mogą podjąć działania. Możesz również ograniczyć monitorowaną skrzynkę pocztową tylko do połowów, które były wcześniej prawidłowymi adresami e-mail. 

Każda Skrzynka pocztowa będzie otrzymywać dobrą okazję do spamu i może ostatecznie wypełnić, jeśli nie jest ściśle monitorowana. (Istnieją limity dotyczące odbierania). 

Jeśli zdecydujesz się kontynuować, wykonaj następujące czynności:

1. Utwórz dynamiczną grupę dystrybucyjną, & dołączyć "wszystkie typy adresatów".

2. Utwórz dedykowaną skrzynkę pocztową do obsługi wiadomości e-mail, na przykład catchall@domain.com.

3. W przypadku określonej domeny ustaw dla tej usługi wartość "InternalRelay". Jeśli później usuniesz przechwycenie, upewnij się, że domena jest ponownie ustawiona na wartość autorytatywna.

4. Utwórz regułę transportu o w następujący sposób:

    - Jeśli nadawca to "spoza organizacji"
    - Przekierowywanie wiadomości do Catchall@domain.com
    - Chyba że adresat jest członkiem allusers@domain.com (grupa dystrybucyjna zawiera wszystkich członków)
    - Sprawdzanie, czy nowe skrzynki pocztowe są dodawane do grupy dystrybucyjnej dynamicznej
