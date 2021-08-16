---
title: Przykład programu Microsoft Defender Office 365 ochrony przed wyłudzaniem informacji
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035016"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Przykład programu Microsoft Defender Office 365 ochrony przed wyłudzaniem informacji

Te ustawienia umożliwiają zasady o nazwie *Domain (Domena) i GENERAL (Dyrektor generalny).* Te zasady zapewniają zarówno ochronę użytkowników, jak i domen przed personifikacji, a następnie dotyczą wszystkich wiadomości e-mail odbieranych przez użytkowników w domenie. Najpierw dodaj następujące informacje, aby utworzyć zasady:

- **Nazwa:** Opis domeny i dyrektora **generalnego:** gwarantuje, że dyrektor generalny i Twoja domena nie są personifikowane.
  **Dotyczy:** Wybierz **domenę adresata to**. W **obszarze Dowolny z nich** wybierz pozycję **Wybierz**, a następnie wybierz domenę. Wybierz **pozycję + Dodaj**. Zaznacz pole wyboru obok nazwy domeny na liście (na przykład *contoso.com*), a następnie wybierz pozycję **Dodaj**. Wybierz **pozycję Gotowe**.
- Po utworzeniu zasad można je dostosować, korzystając z następujących opcji:
  - **Dodawanie użytkowników w celu ochrony:** W tym przykładzie dodaj co najmniej adres e-mail dyrektora generalnego.
  - **Dodawanie domen w celu ochrony**: Dodaj domenę organizacji, która zawiera biuro Dyrektora Generalnego.
  - **Wybierz akcje:** Jeśli wiadomość e-mail jest wysyłana przez spersonifikowanego **użytkownika,** wybierz pozycję Przekieruj wiadomość na inny adres e-mail **,** a następnie wprowadź adres e-mail administratora zabezpieczeń (na przykład *securityadmin@contoso.com).* W **przypadku, gdy wiadomość e-mail jest wysyłana za pomocą personifikacji domeny,** wybierz **pozycję Poddaj wiadomość kwarantannie**.
  - **Inteligencja** skrzynek pocztowych: ta opcja jest domyślnie zaznaczona podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji. Aby uzyskać najlepsze **wyniki, pozostaw** to ustawienie wł.
  - **Dodaj zaufanych nadawców i domeny:** W tym przykładzie nie definiuj żadnych zastępować.
- Po przejrzenia ustawień wybierz pozycję Utwórz **te zasady** lub **Zapisz** odpowiednio do potrzeb.

Aby dowiedzieć się więcej, zobacz [Zasady ochrony przed wyłudzaniem informacji w Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
