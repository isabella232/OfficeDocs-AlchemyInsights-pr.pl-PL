---
title: 2491 Alert o wiadomościach e-mail z zasad "Dostarczono informacje o wiadomościach wyłudowych z powodu zastąpienia dzierżawy lub użytkownika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316368"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertuj wiadomości e-mail z zasad "Dostarczono informacje na temat informacji o wiadomościach na temat wiadomości e-mail z powodu zastąpienia dzierżawy lub użytkownika"

W organizacjach z licencjami Microsoft Defender for Office 365 P1 i P2 są dostępne domyślne zasady alertów o nazwie **Phish Delivered** z powodu zastąpienia dzierżawy lub użytkownika. Jeśli otrzymano ten alert, należy zbadać następujące czynności:

1. W komunikacie alertu kliknij pozycję **Wyświetl alert,** aby przejść do strony **Alerty** w Microsoft 365 Defender sieci Web.

2. Wybierz alert, aby wyświetlić opcję Wyświetl listę wiadomości **lub** **Wyświetl wiadomości w Eksploratorze**. W obu tych opcjach znajdują się szczegóły wiadomości, w tym identyfikator wiadomości. Link Eksplorator zagrożeń automatycznie filtruje wiadomości zgodne z kryteriami alertu. Może być konieczne dostosowanie filtru daty w Eksploratorze zagrożeń.

Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznie skonfigurowanego zastąpienia:

- Dozwolony nadawca lub domena ustawione przez użytkownika.
- Dozwolony nadawca lub domena określone przez administratora w zasadach ochrony przed spamem.
- Dozwolony adres IP w zasadach filtru połączenia.
- Reguła przepływu poczty e-mail (znana również jako reguła transportu) skonfigurowana do zezwalania na przychodzące wiadomości.

Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako wyłudzająca informacje, zgłoś tę wiadomość firmie Microsoft za pomocą przesyłania przez administratora. [](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

Użytkownicy mogą korzystać z dodatku Report Message (Wiadomość raportu) lub dodatku do wyłudzania informacji [(Report Phishing)](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) w programie Outlook przesłać próbki wiadomości do firmy Microsoft.
