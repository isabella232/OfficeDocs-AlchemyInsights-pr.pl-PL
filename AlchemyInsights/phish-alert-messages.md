---
title: Alert (2491) wiadomości e-mail z poziomu "phishing dostarczany z powodu zasad przesłonięcia dzierżawy lub użytkownika"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728621"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alarmowanie wiadomości e-mail z poziomu "phishing dostarczany z powodu zasad przesłonięcia dzierżawy lub użytkownika"

Domyślna zasada alertów o nazwie "wyłudzanie informacji została dostarczona z powodu przesłonięcia dzierżawy lub zastąpienia użytkownika" została przekazana do dzierżawców za pomocą licencji na usługi Office 365 ATP i P2. Jeśli otrzymałeś ten alert, możesz sprawdzić następujące kroki:

1. W oknie komunikatu alertu kliknij pozycję **Wyświetl alert** , aby przejść do strony **alerty** w centrum zabezpieczeń & zgodności.

2. Wybierz Alert, aby zobaczyć opcję **wyświetlania listy wiadomości** lub **wyświetlania wiadomości w Eksploratorze**. W obu tych opcjach przedstawiono szczegóły wiadomości zawierającej identyfikator wiadomości. Pamiętaj, że link w Eksploratorze zagrożeń będzie automatycznie filtrować wiadomości zgodne z kryteriami alertów. Być może trzeba dostosować filtr daty w Eksploratorze zagrożeń.

Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznej konfiguracji przesłonięcia:

- Dozwolony nadawca lub domena ustawiona przez użytkownika.

- Dozwolony nadawca lub domena ustawiona przez administratora w zasadach ochrony przed spamem.

- Dozwolony adres IP w zasadach filtru połączeń.

- Reguła przepływu poczty (nazywana też regułą transportu), która jest skonfigurowana do zezwalania na wiadomości.

Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako wyłudzanie informacji, użyj [dodatku wiadomości raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook, aby przesłać próbki wiadomości do firmy Microsoft.
