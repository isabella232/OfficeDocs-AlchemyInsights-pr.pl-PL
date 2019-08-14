---
title: Wiadomości e-mail alertu 2491 od wykrywanie witryn wyłudzających wydana z powodu dzierżawcę lub użytkownika zastępują zasady
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391436"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Wiadomości e-mail alertu z wykrywanie witryn wyłudzających wydana z powodu dzierżawcę lub użytkownika zastępują zasady

Domyślna zasada alert o nazwie "Wykrywanie witryn wyłudzających dostarczone ze względu na zastąpienie dzierżawcę lub użytkownika" była dostępna dla najemców z licencjami Office 365 ATP P1 i P2. Jeśli otrzymasz ten komunikat, Oto kroki, aby zbadać:

1. Z komunikatu alertu kliknij przycisk **Wyświetl Alert** , aby przejść do strony **alerty** zabezpieczeń & Centrum zgodności.

2. Wybierz ten alert, aby wyświetlić opcję na **liście wiadomości w widoku** lub **Wyświetlanie wiadomości w Eksploratorze**. Obie te opcje przejście do szczegółów wiadomości, która zawiera identyfikator wiadomości. Uwaga: łącze zagrożenie Explorer automatycznie przefiltruje wiadomości, które spełniają kryteria alertu. Konieczne może być dostosowanie filtr daty w Eksploratorze zagrożenie.

Wiadomość wyłudzająca informacje została dostarczona z powodu override ręcznie skonfigurowane:

- Dozwolone nadawcy lub domeny ustawiona przez użytkownika.

- Dozwolonych nadawców lub domeny ustawiona przez administratora w zasadzie zwalczania spamu.

- Dozwolony adres IP w zasadzie filtr połączeń.

- Reguły przepływu poczty (znany również jako regułę transportu), która jest skonfigurowana do obsługi wiadomości w.

Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako pozyskiwać, użyj programu Outlook [dodatek wiadomość raportu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) przedłożenia próbek wiadomości do firmy Microsoft.
