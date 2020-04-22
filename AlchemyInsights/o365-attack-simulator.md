---
title: 2681 Symulator ataku w usłudze Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713476"
---
# <a name="attack-simulator-in-microsoft-365"></a>Symulator ataku w usłudze Microsoft 365

- Brakuje Ci Symulatora Ataku? Symulator ataku wymaga **planu zaawansowanej ochrony przed zagrożeniami usługi Office 365 2 (plan ATP 2)** lub **usługi Office 365 Enterprise E5.** Symulator ataku **nie** jest uwzględniony w planie zaawansowanej ochrony przed zagrożeniami usługi Office 365 1 (plan ATP 1), usłudze Office 365 Enterprise E3 ani w żadnych subskrypcjach aplikacji microsoft 365 dla firm.

- Konto używane do przeprowadzania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego(MFA). Aby uzyskać więcej informacji na temat wymagań symulatora ataku, zobacz [ten temat](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Ważne informacje o symulacjach ataku **Brute Force Password:**

  - Jeśli konto docelowe ma włączone uwierzytelnianie wieloskładnikowe i hasło zostało poprawnie odgadnięty, konto nie będzie wyświetlane jako naruszone (drugi czynnik uwierzytelniania będzie niekompletny).

  - Plik hasła nie może być większy niż 10 MB. Użyj jednego hasła w wierszu i dołącz pusty wiersz (powrót karetki) po ostatnim haśle na liście.

- Ważne informacje o **spear phishingu** dołączyć symulacje:

  - Zgodnie z projektem nie można podać niestandardowej wartości **adresu URL serwera logowania do witryn wyłudzających informacje.**

  - Jeśli adresat używa [dodatku Włącz komunikat o zgłoś,](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) aby zgłosić wiadomość jako wyłudzającą informacje, może nie być wyświetlanych alertów dotyczących wiadomości (ponieważ jest to symulowany atak).

- Raporty: Po zakończeniu symulowanego ataku możesz kliknąć **szczegóły ataku,** aby zobaczyć raport.

- Aby uzyskać szczegółowe instrukcje i nowe funkcje w symulatorze ataku, zobacz [Symulator ataku w usłudze Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
