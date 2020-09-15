---
title: 'Błąd: reguły na tym komputerze nie pasują do siebie.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690973"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Błąd: reguły na tym komputerze nie pasują do siebie.

Aby wyświetlić zaktualizowany stan tego znanego problemu, zobacz [reguły na tym komputerze są niezgodne z regułami w programie Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Zespół programu Outlook zaimplementował poprawkę w kompilacji 12928,10000. Poprawka jest już w Niejawnym programie testów i będzie przełączana do kanału miesięcznego po późnych 2020 czerwca. Po utworzeniu stałej kompilacji możesz wyświetlić monit "które reguły chcesz zachować" po raz ostatni. Wybierz pozycję serwer po wyświetleniu monitu, a następnie wróć do programu Outlook i ponownie Włącz wszystkie reguły, które zostały wyłączone.

Dopóki poprawka nie będzie dostępna, użyj następującego obejścia:

**Obejście**: w przypadku ostatnich raportów wystąpił problem dotyczący utworzonych tylko reguł klientów w aplikacji klasycznej Outlook. Jeśli problem nadal występuje, warto usunąć reguły, a następnie utworzyć i edytować reguły tylko w aplikacji OWA (Outlook Web App) do momentu rozwiązania problemu.

Jeśli nie można usunąć reguł ręcznie, możesz uruchomić polecenie programu Outlook po uruchomieniu programu Outlook, uruchamiając Outlook.exe/cleanrules. Spowoduje to usunięcie zarówno reguł klienta, jak i serwera. Spowoduje to usunięcie wszystkich reguł dla wszystkich kont w profilu programu Outlook. To polecenie jest dokładniej opisane w artykule przełączniki wiersza polecenia.

