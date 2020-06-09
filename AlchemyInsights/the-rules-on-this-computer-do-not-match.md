---
title: 'Błąd: reguły na tym komputerze nie są zgodne'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664256"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Błąd: reguły na tym komputerze nie są zgodne

Aby zobaczyć zaktualizowany stan tego znanego problemu, zobacz [Reguły na tym komputerze nie są zgodne z regułami programu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928.10000. Poprawka jest już w Insider Fast i trafi do Miesięcznego Kanału pod koniec czerwca 2020. Po uzyskaniu stałej kompilacji możesz po raz ostatni otrzymać monit "Które reguły chcesz zachować". Wybierz pozycję Serwer po wyświetleniu monitu, a następnie wróć do programu Outlook i ponownie włącz wszystkie wyłączone reguły.

Dopóki poprawka nie będzie dostępna, użyj następującego obejścia:

**Obejście**: W ostatnich raportach wystąpił problem dla tych, którzy utworzyli tylko reguły klienta na pulpicie programu Outlook. Jeśli nadal występuje problem, należy rozważyć usunięcie reguł, a następnie utworzyć i edytować reguły tylko w programie OWA (Outlook Web App) do momentu rozwiązania problemu.

Jeśli nie można usunąć reguł ręcznie, możesz uruchomić polecenie programu Outlook po uruchomieniu programu Outlook, uruchamiając program Outlook.exe /cleanrules. Spowoduje to usunięcie reguł klienta i serwera. Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook. To polecenie jest dodatkowo udokumentowane w artykule Przełączniki wiersza polecenia.

