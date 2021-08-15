---
title: Identyfikowanie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014910"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identyfikowanie adresu IP i klienta w dziennikach inspekcji

Adres IP odpowiadający działaniu innego użytkownika lub Microsoft 365 jest wyświetlany w dziennikach inspekcji. Rejestrowane są również informacje o kliencie. Poniżej po procedurach identyfikowania takich informacji

1. Zaloguj się do [centrum Microsoft 365 zgodności.](https://protection.office.com/)

2. Przejdź do **strony Przeszukiwanie**  >  **dziennika inspekcji wyszukiwania.**

   Jeśli interesuje Cię określone działanie, wybierz je z **listy Działania.** Jeśli nie, zostaną zwrócone wszystkie działania dla wybranego użytkownika (ustawienie domyślne).

   **Uwaga:** Niektóre działania mogą nie być dostępne w menu **Działania.** jednak te elementy inspekcji zostaną zwrócone, jeśli wybrano opcję Pokaż wyniki dla **wszystkich** działań (ustawienie domyślne).

3. Określ nazwę użytkownika w **polu Użytkownicy,** wybierz odpowiedni zakres dat dla działania, a następnie kliknij pozycję **Wyszukaj**.

W wynikach wyszukiwania zobaczysz adres IP tego działania w okienku wyników. Wybierz rekord inspekcji, aby wyświetlić szczegółowe informacje w **wysuwanych** szczegółach (na przykład Klient, Użytkownik, który wykonał akcję itp.).

Aby uzyskać więcej informacji, zobacz Znajdowanie adresu IP komputera użytego do uzyskania dostępu [do naruszonego konta.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
