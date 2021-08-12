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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061442"
---
# <a name="sensitivity-labels-not-appearing"></a>Etykiety wrażliwości nie są wyświetlane

Etykiety wrażliwości umożliwiają klasyfikowanie i chroninie poufnej zawartości. Można je tworzyć w centrum Centrum zgodności platformy Microsoft 365, Microsoft 365 lub centrum zabezpieczeń Microsoft 365 w & w obszarze Etykiety klasyfikacji > wrażliwości. Aby dowiedzieć się więcej o tej funkcji, zobacz [Omówienie etykiet wrażliwości.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Jeśli etykiety wrażliwości zostały skonfigurowane, ale nie są wyświetlane w Microsoft 365 aplikacji, sprawdź następujące kwestie:

- Upewnij się, że etykieta wrażliwości została [opublikowana](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) dla użytkowników i grup, których chcesz użyć.

- Upewnij się, że użytkownik używa aplikacji obsługującej etykiety wrażliwości — zobacz etykiety wrażliwości [w dokumencie.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Jeśli migrowane są etykiety usługi [Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)należy pamiętać o zagadnieniach wymienionych [tutaj.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Obsługa ochrony przed utratą danych (DLP): Obecnie jako warunku zasad DLP można używać tylko etykiet przechowywania.  Obsługa etykiet wrażliwości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad tym.

- Po włączeniu szyfrowania na etykiecie wrażliwości możesz wybrać jedną z tych opcji:
    - Przypisz uprawnienia teraz
    - Umożliwianie użytkownikom przypisywania uprawnień


Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [Znane problemy dotyczące etykiet wrażliwości.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)