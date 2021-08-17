---
title: Rozwiązywanie typowych problemów z programem Microsoft Defender dla Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898254"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Rozwiązywanie typowych problemów z programem Microsoft Defender dla Office 365

Oto kilka rozwiązań typowych problemów z programem Microsoft Defender dla Office 365:

- **Opóźnienie wiadomości:**

  Opóźnienia w dostarczaniu wiadomości e-mail mogą być spowodowane Sejf załączników wiadomości. Aby uzyskać więcej informacji, [zobacz Sejf ustawienia zasad Załączniki.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Zgłaszanie wyników fałszywie dodatnich lub ujemnych:**

  Aby uzyskać więcej informacji, zobacz [Zgłaszanie wiadomości i plików do firmy Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Włączanie Sejf linku:**

  1. W portalu Microsoft 365 Defender przejdź do sekcji Zasady & e-mail & Zasady zagrożeń Sejf <https://security.microsoft.com/>  \>  \>  \> **linki** **do** zasad.

     Aby przejść bezpośrednio do **strony Sejf,** <https://security.microsoft.com/safelinksv2> użyj .

  2. Na **stronie Sejf** wybierz zasady, klikając nazwę zasad.
  3. W wyświetlonym wysuwanych szczegółach wykonaj jedną z następujących czynności:
     - Aby dodać nowe zasady, wybierz pozycję **+ Utwórz.** Zostanie uruchomienie kreatora, który pomoże Ci zdefiniować ustawienia zasad.
     - Aby edytować istniejące zasady, wybierz je, klikając nazwę zasad. W wyświetlonym wysuwu szczegółów wybierz pozycję **Edytuj** w sekcji **Ustawienia** ochrony.
  4. Na **stronie Ustawienia ochrony** skonfiguruj następujące ustawienia:
     - Włącz Wybierz **akcję dla nieznanych, potencjalnie złośliwych adresów URL w wiadomościach.**
     - Wybierz **pozycję Zastosuj bezpieczne linki do wiadomości wysyłanych w organizacji.**

  Aby uzyskać więcej informacji, [zobacz Konfigurowanie zasad Sejf Linków w programie Microsoft Defender dla systemu Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
