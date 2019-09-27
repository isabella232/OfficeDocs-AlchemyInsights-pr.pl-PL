---
title: Etykiety czułości nie pojawiają się
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207235"
---
# <a name="sensitivity-labels-not-appearing"></a>Etykiety czułości nie pojawiają się

Etykiety czułości pozwalają klasyfikować i chronić poufne treści. Mogą one być tworzone w centrum zgodności Microsoft 365, Centrum zabezpieczeń Microsoft 365 lub Office 365 Security & Compliance Center w obszarze Klasyfikacja etykiet > czułość. Aby dowiedzieć się więcej na temat tej funkcji, zobacz [Omówienie etykiet czułości](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Jeśli skonfigurowano etykiety czułości, ale nie są wyświetlane w aplikacjach pakietu Office, sprawdź następujące elementy:

- Potwierdź, że etykieta czułości została [opublikowana](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) dla użytkowników i grup, które mają.

- Potwierdź, że użytkownik korzysta z aplikacji obsługującej etykiety czułości — zobacz [etykiety czułości w dokumencie](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Jeśli [migrujesz etykiety usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), należy pamiętać o zagadnienia wymienione w [tym miejscu](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Obsługa zapobiegania utracie danych (DLP): obecnie tylko etykiety przechowywania mogą być użyte jako warunek w zasadach DLP.  Obsługa etykiet czułości w zasadach DLP nie jest jeszcze dostępna, ale pracujemy nad nim.

- Gdy szyfrowanie jest włączone na etykiecie czułości, można wybrać opcję:
    - Przypisz uprawnienia teraz
    - Pozwól użytkownikom przypisywać uprawnienia


Aby uzyskać więcej informacji na temat możliwych problemów, zobacz [znane problemy z etykietami czułości](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).