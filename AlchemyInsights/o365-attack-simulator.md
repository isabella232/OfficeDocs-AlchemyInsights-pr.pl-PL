---
title: 2681 symulatora ataków w systemie Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801561"
---
# <a name="attack-simulator-in-microsoft-365"></a>Symulator ataków w systemie Microsoft 365

- Czy brakuje symulatora ataku? Symulator ataków wymaga **programu Microsoft Defender for Office 365 plan 2 (ATP plan 2)** lub **Office 365 Enterprise E5** . Aplikacja symulatora ataków **nie** jest uwzględniona w usłudze Microsoft Defender dla pakietu Office 365 plan 1 (plan ATP 1), Office 365 Enterprise E3 ani żadnych aplikacji Microsoft 365 dla subskrypcji biznesowych.

- Konto używane do uruchamiania symulowanych ataków wymaga uprawnień administratora globalnego lub administratora zabezpieczeń oraz uwierzytelniania wieloskładnikowego (MFA). Aby uzyskać więcej informacji na temat wymagań dotyczących ataków na ataki, zobacz [ten temat](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Ważne zagadnienia związane z symulacją ataków za ataki za pośrednictwem **hasła** :

  - Jeśli dla konta docelowego jest włączone uwierzytelnianie wieloskładnikowe, a hasło zostało nagrane poprawnie, konto nie będzie widoczne jako zagrożone (drugi współczynnik uwierzytelniania będzie niekompletny).

  - Rozmiar pliku hasła nie może przekraczać 10 MB. Użyj jednego hasła na wiersz i Dołącz pusty wiersz (znak powrotu karetki) po ostatnim haśle na liście.

- Ważne zagadnienia dotyczące **Spearych informacji** o dołączaniu do witryn wyłudzających informacje:

  - Według projektu nie można podać wartości niestandardowej dla **adresu URL serwera logowania wyłudzających informacje** .

  - Jeśli odbiorca używa [dodatku Włącz wiadomość raportu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , aby zgłosić wiadomość jako wyłudzanie informacji, użytkownik może nie otrzymywać alertów dotyczących wiadomości (ponieważ jest to symulowane ataki).

- Raporty: po zakończeniu symulowanego ataku można kliknąć pozycję **szczegóły ataku** , aby wyświetlić raport.

- Szczegółowe instrukcje i nowe funkcje w symulatorze ataku znajdziesz [w witrynie Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
