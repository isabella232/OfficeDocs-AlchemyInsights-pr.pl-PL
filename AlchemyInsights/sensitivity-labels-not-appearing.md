---
title: Etykiety wrażliwości nie są wyświetlane
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801194"
---
# <a name="sensitivity-labels-not-appearing"></a>Etykiety wrażliwości nie są wyświetlane

Etykiety wrażliwości pozwalają sklasyfikować i chronić poufną zawartość. Można je utworzyć w centrum zgodności z programem Microsoft 365, Centrum zabezpieczeń Microsoft 365 lub Microsoft 365 Security & Center w obszarze Klasyfikacja wrażliwości > etykiet. Aby dowiedzieć się więcej o tej funkcji, zobacz [Omówienie etykiet wrażliwości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Jeśli etykiety wrażliwości zostały skonfigurowane, ale nie są wyświetlane w aplikacjach Microsoft 365, sprawdź następujące elementy:

- Upewnij się, że etykieta wrażliwości została [opublikowana](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) na potrzeby użytkowników i grup.

- Upewnij się, że użytkownik korzysta z aplikacji obsługującej etykiety wrażliwości — zobacz [etykiety liter w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Jeśli [przeprowadzasz migrację etykiet ochrony danych platformy Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), zapoznaj się z wymienionymi [tutaj](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)uwagami.

- Obsługa ochrony przed utratą danych (DLP): obecnie w zasadach DLP można użyć tylko etykiet przechowywania jako warunków.  Obsługa etykiet wrażliwości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad nią.

- Po włączeniu szyfrowania na etykiecie czułości możesz wybrać jedną z następujących opcji:
    - Przydziel teraz uprawnienia
    - Zezwalanie użytkownikom na przypisywanie uprawnień


Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).