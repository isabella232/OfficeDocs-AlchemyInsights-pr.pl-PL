---
title: 2491 Alert wiadomości e-mail z "Phish dostarczone z powodu dzierżawy lub zastąpienia użytkownika" zasady
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758939"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alert wiadomości e-mail z "Phish dostarczone z powodu dzierżawy lub zastąpienia użytkownika" zasady

Domyślna zasada alertów o nazwie "Phish delivered due to tenant or user override" została wdrożona dla dzierżaw z licencjami Office 365 ATP P1 i P2. Jeśli ten alert został odebrany, oto kroki, które należy zbadać:

1. W komunikacie alertu kliknij pozycję **Wyświetl alert,** aby przejść do strony **Alerty** w Centrum zgodności & zabezpieczeń.

2. Wybierz alert, aby wyświetlić opcję **Wyświetl listę wiadomości** lub Wyświetl wiadomości w **Eksploratorze**. Obie te opcje przejmują cię do szczegółów wiadomości, która zawiera identyfikator wiadomości. Należy zauważyć, że łącze Eksploratora zagrożeń będzie automatycznie filtrować wiadomości zgodne z kryteriami alertu. Może być konieczne dostosowanie filtru daty w Eksploratorze zagrożeń.

Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznie skonfigurowanego zastąpienia:

- Dozwolony nadawca lub domena ustawiona przez użytkownika.

- Dozwolony nadawca lub domena ustawiona przez administratora w zasadach antyspamowych.

- Dozwolony adres IP w zasadach filtrowania połączeń.

- Reguła przepływu poczty (znana również jako reguła transportu), która jest skonfigurowana tak, aby zezwalać na wysyłanie wiadomości.

Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako phish, użyj [dodatku Wiadomości raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook, aby przesłać przykłady wiadomości do firmy Microsoft.
