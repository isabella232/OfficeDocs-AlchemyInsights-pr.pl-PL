---
title: 2491 Alert o wiadomościach e-mail z zasad "Dostarczono informacje o wiadomościach phish z powodu zastąpienia dzierżawy lub użytkownika"
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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999682"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alert w wiadomościach e-mail z zasad "Dostarczono informacje na temat informacji o wiadomościach na temat wiadomości e-mail z powodu zastąpienia dzierżawy lub użytkownika"

W dzierżawach usługi Microsoft Defender dla komputerów Office 365 P1 i P2 w dzierżawie zostały włączone domyślne zasady alertów o nazwie "Dostarczono phish z powodu zastąpienia dzierżawy" Jeśli otrzymano ten alert, należy zbadać następujące czynności:

1. W komunikacie alertu kliknij pozycję **Wyświetl alert,** aby przejść do strony **Alerty** w Centrum & zabezpieczeń.

2. Wybierz alert, aby wyświetlić opcję Wyświetl **listę wiadomości lub** Wyświetl wiadomości w **Eksploratorze**. W obu tych opcjach znajdują się szczegóły wiadomości, w tym identyfikator wiadomości. Link Eksplorator zagrożeń automatycznie filtruje wiadomości zgodne z kryteriami alertu. Może być konieczne dostosowanie filtru daty w Eksploratorze zagrożeń.

Wiadomość wyłudzająca informacje została dostarczona z powodu ręcznie skonfigurowanego zastąpienia:

- Dozwolony nadawca lub domena ustawione przez użytkownika.

- Dozwolony nadawca lub domena określone przez administratora w zasadach ochrony przed spamem.

- Dozwolony adres IP w zasadach filtru połączenia.

- Reguła przepływu poczty e-mail (znana również jako reguła transportu), która jest skonfigurowana do zezwalania na przychodzące wiadomości.

Jeśli uważasz, że wiadomość została niepoprawnie oznaczona jako phish, użyj dodatku Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) (Wiadomość raportu) w celu przesłania przykładowych wiadomości do firmy Microsoft.
