---
title: Tworzenie wiadomości e-mail catch wszystkich
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286202"
---
# <a name="create-an-email-catch-all"></a>Tworzenie wiadomości e-mail catch wszystkich

Korzystanie z połowu wszystko jest zdecydowanie odradzane. Lepiej jest zapewnić odbicie z powrotem do nadawcy, informując nadawców, że ich wiadomość nie może zostać dostarczona jako adresowana, aby mogli podjąć działania. Można również ograniczyć monitorowana skrzynka pocztowa, aby tylko wyłapywać wcześniej prawidłowe adresy e-mail. 

Każdy połów wszystkie skrzynki pocztowej otrzyma sporo spamu i może ostatecznie wypełnić, jeśli nie ściśle monitorowane. (Istnieją limity odbioru.) 

Jeśli zdecydujesz się kontynuować, wykonaj następujące kroki:

1. Utwórz dynamiczną grupę dystrybucyjną & zawierać "Wszystkie typy adresatów".

2. Utwórz dedykowaną skrzynkę pocztową, aby wyłapywać wiadomości e-mail, na przykład catchall@domain.com.

3. W przypadku określonej domeny ustaw DomainType na "InternalRelay". Jeśli później usuniesz wszystkie catch, należy ustawić domenę z powrotem do autorytatywne.

4. Utwórz regułę transportu przepływów mailowych w następujący sposób:

    - Jeśli nadawca jest "Poza organizacją"
    - Przekieruj wiadomość do Catchall@domain.com
    - Z wyjątkiem sytuacji, gdy odbiorca jest członkiem allusers@domain.com (Grupa dystrybucyjna zawiera wszystkich członków)
    - Upewnij się, że nowe skrzynki pocztowe są dodawane do dynamicznej grupy dystrybucyjnej
