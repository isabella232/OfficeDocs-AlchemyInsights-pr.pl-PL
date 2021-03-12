---
title: Automatyczne szyfrowanie wiadomości e-mail usługi Office 365 wysyłanych do określonych domen
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749305"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatyczne szyfrowanie wiadomości e-mail usługi Office 365 wysyłanych do określonych domen

1. W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz pozycję **przepływ poczty > reguły**. 
2. Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości i ochronę praw do wiadomości w usłudze **Office 365.**
3. W **imieniu** użytkownika wprowadź nazwę reguły, na przykład Szyfruj *wiadomości wysyłane do contoso.com.*
4. W **edycie Zastosuj tę regułę, jeśli** wybierz pozycję **> domeną jest**. 
5. Wprowadź nazwę domeny, na przykład **contoso.com.**
6. Kliknij **ikonę Dodaj (+),** a następnie kliknij przycisk **OK.**
7. Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**. 
8. W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.** (Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania. Ale możesz je dodać!)
9. Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).
10. Kliknij przycisk **Zapisz**.

> [!IMPORTANT]
> Zawsze możesz wrócić i edytować tę regułę później.

Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty w celu szyfrowania wiadomości e-mail [w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)