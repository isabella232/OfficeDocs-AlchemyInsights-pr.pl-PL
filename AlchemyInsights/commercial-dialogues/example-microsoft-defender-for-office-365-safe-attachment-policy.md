---
title: Przykład zasad bezpiecznego załącznika w usłudze Microsoft Defender dla usługi Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749201"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Przykład zasad bezpiecznego załącznika w usłudze Microsoft Defender dla usługi Office 365

Te ustawienia umożliwiają obsługę zasad o nazwie *Bez* opóźnień, która natychmiast dostarcza wiadomości, a następnie ponownie podłącza załączniki po ich zeskanowaniu:

- **Nazwa:** Brak opóźnień
- **Opis:** Natychmiast dostarcza wiadomości i ponownie podłącza załączniki po zeskanowaniu.
- **Odpowiedź:** Wybierz opcję **Dostarczanie dynamiczne.** Aby uzyskać więcej informacji, zobacz [Dynamiczne dostarczanie w zasadach bezpiecznych załączników.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Przekieruj** sekcję załączników: Wybierz opcję Włącz przekierowywanie **,** a następnie wprowadź adres e-mail administratora globalnego platformy Microsoft 365, administratora zabezpieczeń lub analityka zabezpieczeń, który będzie badać złośliwe załączniki.
- **Sekcja Zastosowano** do: Wybierz **pozycję Domena adresata to**, a następnie wybierz domenę. Wybierz **pozycję dodaj**, a następnie wybierz przycisk **OK.** Po zakończeniu wybierz pozycję **Zapisz**.

Aby dowiedzieć się więcej, zobacz [Bezpieczne załączniki w programie Microsoft Defender dla usługi Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
