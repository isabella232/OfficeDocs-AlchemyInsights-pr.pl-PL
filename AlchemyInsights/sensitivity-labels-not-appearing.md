---
title: Etykiety czułości nie są wyświetlane
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581025"
---
# <a name="sensitivity-labels-not-appearing"></a>Etykiety czułości nie są wyświetlane

Etykiety czułości umożliwiają klasyfikowanie i ochronę poufnych treści. Można je tworzyć w centrum zgodności usługi Microsoft 365, centrum zabezpieczeń usługi Microsoft 365 lub centrum zgodności & zabezpieczeń usługi Microsoft 365 w obszarze Etykiety klasyfikacji > czułości. Aby dowiedzieć się więcej o tej funkcji, zobacz [Omówienie etykiet czułości](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Jeśli etykiety czułości zostały skonfigurowane, ale nie są one wyświetlane w aplikacjach usługi Microsoft 365, sprawdź następujące kwestie:

- Upewnij się, że etykieta czułości została [opublikowana](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) dla użytkowników i grup, które chcesz.

- Upewnij się, że użytkownik korzysta z aplikacji obsługującej etykiety czułości — zobacz [etykiety czułości w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Jeśli [przeprowadzasz migrację etykiet usługi Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)należy pamiętać o zagadnieniach wymienionych [tutaj](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Obsługa zapobiegania utracie danych (DLP): obecnie tylko etykiety przechowywania mogą być używane jako warunek w zasadach DLP.  Obsługa etykiet czułości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad tym.

- Gdy szyfrowanie jest włączone na etykiecie czułości, można wybrać:
    - Przypisz uprawnienia teraz
    - Zezwalanie użytkownikom na przypisywanie uprawnień


Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [Znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).