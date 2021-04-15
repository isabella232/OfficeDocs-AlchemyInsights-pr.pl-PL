---
title: 'Błąd: Reguły na tym komputerze nie są zgodne'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782962"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Błąd: Reguły na tym komputerze nie są zgodne

Aby wyświetlić zaktualizowany stan tego znanego problemu, zobacz Reguły na tym komputerze nie są zgodne z [regułami w programie Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928.10000. Poprawka jest już dostępna w niejawnym programie testów w szybkich wersjach i trafi do kanału miesięcznego pod koniec czerwca 2020 r. Po naprawieniu kompilacji może ostatni raz zostać wyświetlony monit "Które reguły chcesz zachować". Po wyświetleniu monitu wybierz pozycję Serwer, a następnie wróć do programu Outlook i ponownie włącz reguły, które zostały wyłączone.

Do czasu, aż poprawka będzie dostępna, użyj następującego obejścia:

**Obejście:** W ostatnich raportach problem pojawił się u tych osób, które tylko tworzyły reguły klienta w klasycznej wersji programu Outlook. Jeśli problem nadal występuje, rozważ usunięcie reguł, a następnie utworzenie i edytowanie reguł tylko w aplikacji OWA (Outlook Web App), dopóki problem nie zostanie rozwiązany.

Jeśli nie możesz ręcznie usunąć reguł, możesz uruchomić polecenie programu Outlook podczas uruchamiania programu Outlook, uruchamiając polecenie Outlook.exe /cleanrules. Spowoduje to usunięcie zarówno reguł klienta, jak i reguł serwera. Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook. To polecenie jest dodatkowo udokumentowane w artykule Przełączniki wiersza polecenia.

