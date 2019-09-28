---
title: 2681 symulator ataku w pakiecie Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305341"
---
# <a name="attack-simulator-in-office-365"></a>Symulator ataku w pakiecie Office 365

- Czy brakuje symulatora ataku? Symulator ataku wymaga **pakietu office 365 zaawansowane zagrożenie ochrony plan 2 (ATP plan 2)** lub **Office 365 Enterprise E5**. Symulator ataku **nie** jest uwzględniony w pakiecie Office 365 zaawansowane zagrożenie ochrony plan 1 (plan ATP 1), Office 365 Enterprise E3 lub wszelkie subskrypcje Office 365 Business.

- Konto używane do uruchamiania symulowanych ataków wymaga administratora globalnego lub uprawnienia administratora zabezpieczeń i uwierzytelnianie wieloskładnikowe (MFA). Aby uzyskać więcej informacji na temat wymagań symulator ataku Zobacz w [tym temacie](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Ważne rzeczy, o których warto wiedzieć o **Brute Force hasło** ataku symulacje:

  - Jeśli konto docelowe ma włączoną usługę MFA i hasło zostało odgadnięte poprawnie, konto nie będą wyświetlane jako zagrożone (drugi współczynnik uwierzytelniania będzie niekompletna).

  - Plik haseł nie może być większy niż 10 MB. Użyj jednego hasła w wierszu i Dołącz pusty wiersz (powrót karetki) po ostatnim hasło na liście.

- Ważne informacje o symulacjach dołączania **włóczni do phishingu** :

  - Według projektu nie można podać niestandardowej wartości **adresu URL serwera logowania phishingowego**.

  - Jeśli odbiorca używa [Włącz dodatek raportu Raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , aby zgłosić wiadomość jako phishing, może nie odbierać alerty dla wiadomości (ponieważ jest to symulowany atak).

- Raporty: po zakończeniu symulowanego ataku możesz kliknąć pozycję **szczegóły ataku** , aby wyświetlić raport.

- Aby uzyskać szczegółowe instrukcje i nowe funkcje w symulatorze ataku, zobacz [symulator ataku w pakiecie Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
