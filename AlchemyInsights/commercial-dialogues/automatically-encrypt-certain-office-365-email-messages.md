---
title: Automatyczne szyfrowanie niektórych wiadomości e-mail usługi Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749440"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatyczne szyfrowanie niektórych wiadomości e-mail usługi Office 365

Wiadomości wysyłane przez użytkowników do określonych osób zewnętrznych lub organizacji mogą być automatycznie szyfrowane. W tym celu wykonaj następujące czynności:

1. W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz pozycję **przepływ poczty > reguły**. 
2. Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości i ochronę praw do wiadomości w usłudze **Office 365.**
3. W **imieniu** użytkownika wprowadź nazwę reguły, na przykład Szyfruj *wiadomości wysyłane do DrToniRamos@gmail.com*.
4. W **edycie Zastosuj tę regułę, jeśli** wybierz pozycję **Adresatem > jest ta osoba**. 
5. W **oknie Wybieranie** członków wybierz imię i nazwisko osoby, której chcesz użyć reguły szyfrowania, a następnie kliknij pozycję **dodaj**. 
6. Po dodaniu użytkowników kliknij przycisk **OK.**
7. Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**. 
8. W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.** (Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania. Ale możesz je dodać!)
9. Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).
10. Kliknij przycisk **Zapisz**.

> [!IMPORTANT]
> Zawsze możesz wrócić i edytować tę regułę później.

Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty e-mail w celu szyfrowania wiadomości e-mail [w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

