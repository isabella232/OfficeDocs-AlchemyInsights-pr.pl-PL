---
title: Przykład zasad bezpiecznego załącznika usługi Microsoft Defender dla usługi Office 365
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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695181"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Przykład zasad bezpiecznego załącznika usługi Microsoft Defender dla usługi Office 365

Te ustawienia umożliwiają zasady o nazwie *Bez* opóźnień, które natychmiastowo odbierają wiadomości, a następnie ponownie podają załączniki po ich zeskanowaniu:

- **Nazwa:** Brak opóźnień
- **Opis:** natychmiast dostarcza wiadomości i ponownie podłącza załączniki po zeskanowaniu.
- **Odpowiedź:** wybierz opcję **Dostarczanie** dynamiczne. Aby uzyskać więcej informacji, zobacz [dynamiczne dostarczanie w zasadach bezpiecznych załączników.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Przekieruj** sekcję załączników: Wybierz opcję Włącz przekierowywanie, a następnie wprowadź adres e-mail administratora globalnego platformy Microsoft 365, administratora zabezpieczeń lub analityka zabezpieczeń, który będzie badać złośliwe załączniki.
- **Sekcja Zastosowane** do: **Wybierz domenę adresata,** a następnie wybierz domenę. Wybierz **pozycję Dodaj,** a następnie wybierz **przycisk OK.** Po zakończeniu wybierz pozycję **Zapisz.**

Aby dowiedzieć się więcej, zobacz [bezpieczne załączniki w usłudze Microsoft Defender dla usługi Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
