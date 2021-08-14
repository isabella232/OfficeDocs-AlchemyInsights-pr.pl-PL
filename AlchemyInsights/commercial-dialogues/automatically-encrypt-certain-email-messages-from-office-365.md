---
title: Automatyczne szyfrowanie określonych wiadomości e-mail z usługi Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988845"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatyczne szyfrowanie określonych wiadomości e-mail z usługi Office 365

1. W centrum [Exchange wybierz](https://outlook.office365.com/ecp/)pozycję **przepływ poczty e-mail > reguły**. 
2. Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję **Zastosuj Szyfrowanie wiadomości usługi Office 365 ochrony praw do wiadomości**.
3. W **imieniu** użytkownika wprowadź nazwę reguły, na przykład *Zaszyfruj wszystkie wiadomości.*
4. W **przycisku Zastosuj tę regułę, jeśli** wybierz pozycję **[Zastosuj do wszystkich wiadomości]**. 
5. Obok pola **Wykonaj następujące czynności** kliknij pozycję Wybierz **jeden**. 
6. W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj**, a następnie kliknij przycisk **OK.** (Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania. Ale możesz je dodać!)
7. Zaznacz pole **wyboru Prze inspekcji tej reguły z poziomem** ważności, a następnie wybierz odpowiedni poziom. Jeśli Twoja firma ma zobowiązania kontraktowe do wysyłania wszystkich zaszyfrowanych wiadomości e-mail, zalecamy ustawienie na poziomie **Wysoki**.
8. W **obszarze Wybierz model dla tej reguły** kliknij pozycję **Wymusz**. 
9. Wybierz dowolne opcjonalne zaznaczenie (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele może zostać pozostawione domyślnym ustawieniem prostoty).
10. Kliknij **Zapisz**.

> [!IMPORTANT]
> Zawsze możesz wrócić i edytować tę regułę później.

Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty w celu szyfrowania wiadomości [e-mail w Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

