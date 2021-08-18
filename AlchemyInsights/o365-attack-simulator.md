---
title: 2681 Attack Podczas Microsoft 365
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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325081"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Pochoć w Microsoft 365

- Czy brakuje Ci ataku? Atak Podczas ataków Do programu **Microsoft Defender Office 365 plan 2** lub Office 365 Enterprise **E5.** Ataki Dla **usług** Microsoft Defender 1, E3 i E3 nie są uwzględnione w programie Microsoft Defender Office 365 plan 1, Office 365 Enterprise E3 ani żadnych Aplikacje Microsoft 365 dla firm subskrypcji.

- Konto służące do rozpoczynania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego (MFA). Aby uzyskać więcej informacji na temat wymagań dotyczących ataków, zobacz [ten temat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Ważne informacje na temat symulacyjnych **ataków na wymuszanie** haseł:

  - Jeśli dla konta docelowego włączono uwierzytelnianie MFA i hasło zostało odgadane poprawnie, konto nie będzie wyświetlane jako naruszone (drugi współczynnik uwierzytelniania będzie niekompletny).

  - Plik hasła nie może być większy niż 10 MB. Użyj jednego hasła w wierszu i uwzględnij pusty wiersz (powrót karetki) po ostatnim hasłem na liście.

- Ważne informacje na temat symulacyjnych dołączania **wiadomości wyłudzających** informacje:

  - Domyślnie nie można podać niestandardowej wartości adresu URL serwera **logowania wyłudzania informacji.**

  - Jeśli adresat użyje dodatku [Włącz](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) dla wiadomości raportu w celu zgłoszenia tej wiadomości jako próby wyłudzenia informacji, alerty dotyczące wiadomości mogą nie być odbierane (ponieważ jest to symulowany atak).

- Raporty: Po zakończeniu symulowanego ataku możesz kliknąć pozycję **Szczegóły** ataków, aby wyświetlić raport.

- Aby uzyskać szczegółowe instrukcje i nowe funkcje w programie Attack Podczas tego ataku, zobacz [Temat ataków w programie Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
