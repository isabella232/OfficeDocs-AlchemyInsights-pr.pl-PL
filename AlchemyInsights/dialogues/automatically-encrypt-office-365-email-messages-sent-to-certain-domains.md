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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526693"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatyczne szyfrowanie wiadomości e-mail usługi Office 365 wysyłanych do określonych domen

1. W centrum [administracyjnym programu Exchange](https://outlook.office365.com/ecp/)wybierz przepływ **poczty e-mail > reguły.** 
2. Kliknij **ikonę Nowy (+),** a następnie kliknij pozycję Zastosuj szyfrowanie wiadomości usługi **Office 365** i ochronę praw do wiadomości.
3. W **nazwie** wprowadź nazwę reguły, na przykład Szyfrowanie wiadomości *wysyłanych do* contoso.com.
4. W **opcji Zastosuj tę regułę, jeśli** wybierz pozycję Adresat > **domeną.** 
5. Wprowadź nazwę domeny, na przykład **contoso.com.**
6. Kliknij **ikonę Dodaj (+),** a następnie kliknij przycisk **OK.**
7. Obok pola **Wykonaj następujące czynności** kliknij pozycję **Wybierz.** 
8. W menu **rozwijaym szablonu RMS** wybierz pozycję **Szyfruj,** a następnie kliknij przycisk **OK.** (Jeśli nie widzisz tej opcji, oznacza to, że Twój plan nie zawiera automatycznego szyfrowania. Ale możesz go dodać!)
9. Wybierz dowolną opcję opcjonalną (z listy opcji opcjonalnych, które można wybrać w tym momencie, z których wiele można zostawić przy ustawieniu domyślnym dla prostoty).
10. Kliknij przycisk **Zapisz**.

> [!IMPORTANT]
> Zawsze możesz wrócić i edytować tę regułę później.

Aby uzyskać więcej informacji na temat tworzenia reguł szyfrowania, zobacz Definiowanie reguł przepływu poczty e-mail w celu szyfrowania wiadomości e-mail [w usłudze Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)