---
title: Identyfikowanie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716398"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identyfikowanie adresu IP i klienta w dziennikach inspekcji

Adres IP odpowiadający działaniu użytkownika lub administratora usługi Microsoft 365 jest wyświetlany w dziennikach inspekcji. Informacje o kliencie są również rejestrowane. Oto kroki, aby zidentyfikować takie informacje

1. Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/).

2. Przejdź do strony**wyszukiwania dziennika inspekcji** **wyszukiwania.** > 

   Jeśli jesteś zainteresowany określonym działaniem, wybierz je z listy **Działania.** Jeśli nie, wszystkie działania zostaną zwrócone dla wybranego użytkownika (ustawienie domyślne).

   **Uwaga:** Niektóre działania mogą nie być dostępne w menu **Działania;** jednak te elementy inspekcji zostaną zwrócone, jeśli **wybrano opcję Pokaż wyniki dla wszystkich działań** (ustawienie domyślne).

3. Określ nazwę użytkownika w polu **Użytkownicy,** wybierz odpowiedni zakres dat dla działania, a następnie kliknij przycisk **Wyszukaj**.

W wynikach można zobaczyć adres IP dla tego działania w okienku wyników. Wybierz rekord inspekcji, aby wyświetlić szczegółowe informacje w wysu wysu **wysu** wysuwu Szczegóły (na przykład Klient, Użytkownik, który wykonał akcję itp.).

Aby uzyskać więcej informacji, zobacz [Znajdowanie adresu IP komputera używanego do uzyskiwania dostępu do konta, którego bezpieczeństwo zostało naruszone.](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
