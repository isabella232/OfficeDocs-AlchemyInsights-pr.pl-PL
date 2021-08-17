---
title: 2681 Attack W Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895801"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Pochoć w Microsoft 365

- Czy brakuje Ci ataku? Ataki dla systemu Wymaga programu **Microsoft Defender dla Office 365 Plan 2** lub **E5 Office 365 Enterprise E5.** Ataki Nie są **uwzględnione w** programie Microsoft Defender dla Office 365 Plan 1, Office 365 Enterprise E3 ani żadnych innych Aplikacje Microsoft 365 dla firm subskrypcji.

- Konto służące do rozpoczynania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego (MFA). Aby uzyskać więcej informacji na temat wymagań dotyczących ataków, zobacz [ten temat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Ważne informacje na temat symulacyjnych **ataków na wymuszanie** haseł:

  - Jeśli dla konta docelowego włączono uwierzytelnianie MFA i hasło zostało odgadane poprawnie, konto nie będzie wyświetlane jako naruszone (drugi współczynnik uwierzytelniania będzie niekompletny).

  - Plik hasła nie może być większy niż 10 MB. Użyj jednego hasła w wierszu i uwzględnij pusty wiersz (powrót karetki) po ostatnim hasłem na liście.

- Ważne informacje na temat symulacyjnych dołączania **wiadomości wyłudzających** informacje:

  - Domyślnie nie można podać niestandardowej wartości adresu URL serwera **logowania wyłudzania informacji.**

  - Jeśli adresat użyje dodatku [Włącz](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) dla wiadomości raportu w celu zgłoszenia tej wiadomości jako próby wyłudzenia informacji, alerty dotyczące wiadomości mogą nie być odbierane (ponieważ jest to symulowany atak).

- Raporty: Po zakończeniu symulowanego ataku możesz kliknąć pozycję **Szczegóły** ataków, aby wyświetlić raport.

- Aby uzyskać szczegółowe instrukcje i nowe funkcje w programie Attack Podczas tego ataku, zobacz [Temat ataków w programie Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
