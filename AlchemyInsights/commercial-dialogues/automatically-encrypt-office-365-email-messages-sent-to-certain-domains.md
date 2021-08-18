---
title: Automatyczne szyfrowanie Office 365 e-mail wysyłanych do określonych domen
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
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318858"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatyczne szyfrowanie Office 365 e-mail wysyłanych do określonych domen

1. W centrum [Exchange administracyjnego](https://outlook.office365.com/ecp/)wybierz pozycję **przepływ poczty e-mail > reguły**. 
2. Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj Szyfrowanie wiadomości usługi Office 365 ochrony praw **do wiadomości.**
3. W **imieniu** użytkownika wprowadź nazwę reguły, na przykład Szyfruj *wiadomości wysyłane do contoso.com.*
4. W **edycie Zastosuj tę regułę, jeśli** wybierz **pozycję Adresatem > domeną jest**. 
5. Wprowadź nazwę domeny, na przykład **contoso.com**.
6. Kliknij **ikonę Dodaj (+),** a następnie kliknij przycisk **OK.**
7. Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**. 
8. W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.** (Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania. Ale możesz je dodać!)
9. Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).
10. Kliknij **Zapisz**.

**Ważne:** zawsze możesz wrócić i edytować tę regułę później.

Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty w celu szyfrowania wiadomości [e-mail w Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)