---
title: Skrzynka pocztowa otrzymująca wymuszanie ograniczenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316039"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Skrzynka pocztowa otrzymująca wymuszanie ograniczenia

Firma Microsoft niedawno rozpoczęła wymuszanie progu 3600 wiadomości dla skrzynki pocztowej na godzinę. Aby uzyskać więcej informacji, [zobacz Exchange Online limity](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365, które odbierają ponad 3600 wiadomości w ciągu godziny, są ograniczane na następne 60 minut. 

Ponadto limit par nadawców-adresatów (SRP) blokuje wiadomości odbierane przez Microsoft 365 pocztowej od określonego nadawcy. Jeśli pojedynczy nadawca wyśle do określonego adresata ponad 33% progu całkowitego lub 1200 wiadomości na godzinę do określonego adresata, zostanie automatycznie wyliczenie limitu SRP, a skrzynka pocztowa nie będzie akceptować wiadomości od tego nadawcy. Zwróć uwagę, że:

- Ten limit dotyczy wiadomości e-mail otrzymanych od innych dzierżawców, nadawców lokalnych lub internetowych.
- Dostarczanie wiadomości e-mail do skrzynki pocztowej jest blokowane na następne 60 minut. 
- Nadawcy do tych skrzynek pocztowych otrzymują raport o niedo dostarczenia (5.2.121 lub 5.2.122) informujący, że skrzynka pocztowa przekroczyła próg dostarczenia. Poczta wewnątrz dzierżawy (w obrębie tej samej dzierżawy) nadal będzie dostarczana.
- Po zastosowaniu limitu SRP odbierana skrzynka pocztowa nadal przyjmuje wiadomości od innych nadawców.

Administratorzy mogą monitorować bieżącą aktywność skrzynki pocztowej, uzyskujejąc dostęp do nowego raportu i szczegółowych informacji w centrum administracyjnym usługi Exchange o nazwie "Skrzynki pocztowe przekraczające limity adresatów". Szczegółowe informacje są wyświetlane tylko wtedy, gdy dzierżawca ma obrażające skrzynki pocztowe, a raport zawsze pojawia się na pulpicie nawigacyjnym, ale jest pusty, chyba że dzierżawa obrazi skrzynki pocztowe.

Aby uzyskać więcej informacji na temat otrzymywania limitów, zobacz Informacje dotyczące skrzynek pocztowych przekraczających limity w nowej aplikacji [EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Aby uzyskać więcej informacji na temat raportu o przekroczeniu limitów odbiorczych, zobacz Raport o skrzynkach pocztowych przekraczających limity odbierania [w nowym Raporcie EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)