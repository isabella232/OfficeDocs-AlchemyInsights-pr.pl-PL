---
title: Przykład zasad ochrony przed wyłudzaniem informacji w usłudze Microsoft Defender dla usługi Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695646"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Przykład zasad ochrony przed wyłudzaniem informacji w usłudze Microsoft Defender dla usługi Office 365

Te ustawienia umożliwiają zasady o *nazwach Domain (Domena) i DYREKTORA GENERALNEGO (Domain ) (Domena) i GENERALNA (Dyrektor ds. domeny).* Te zasady zapewniają zarówno ochronę użytkowników, jak i domen przed personifikacjami, a następnie dotyczą wszystkich wiadomości e-mail odbieranych przez użytkowników w domenie. Najpierw dodaj następujące informacje, aby utworzyć zasady:

- **Nazwa:** Opis domeny i dyrektora **generalnego:** zapewnia, że dyrektor zarządzający i Twoja domena nie są personifikowane.
  **Zastosowane do:** Wybierz **domenę adresata.** W **obszarze Dowolna z tych** opcji wybierz pozycję **Wybierz,** a następnie wybierz domenę. Wybierz **pozycję +Dodaj.** Zaznacz pole wyboru obok nazwy domeny na liście (na przykład *contoso.com),* a następnie wybierz pozycję **Dodaj.** Wybierz **pozycję Gotowe.**
- Po utworzeniu zasad możesz je dostosować, korzystając z następujących opcji:
  - **Dodaj użytkowników, aby chronić:** W tym przykładzie dodaj co najmniej adres e-mail dyrektora generalnego.
  - **Dodawanie domen w celu ochrony:** Dodaj domenę organizacji, która zawiera biuro dyrektora generalnego.
  - **Wybierz akcje:** Jeśli wiadomość e-mail jest wysyłana przez personifikatora, wybierz pozycję Przekieruj wiadomość na inny adres e-mail, a następnie wprowadź adres e-mail administratora *zabezpieczeń*(na przykład securityadmin@contoso.com). W **przypadku, gdy wiadomość e-mail jest wysyłana przez spersonifikowane domeny,** wybierz pozycję **Poddaj wiadomość kwarantannie.**
  - **Funkcje analizy skrzynki** pocztowej: domyślnie ta opcja jest zaznaczona podczas tworzenia nowych zasad ochrony przed wyłudzaniem informacji. Pozostaw to ustawienie **wł.,** aby uzyskać najlepsze wyniki.
  - **Dodaj zaufanych nadawców i domeny:** W tym przykładzie nie należy definiować żadnych zastępować.
- Po przejrzenia ustawień wybierz pozycję **Utwórz te** zasady lub **Zapisz** odpowiednio do potrzeb.

Aby dowiedzieć się więcej, zobacz zasady ochrony przed [wyłudzaniem informacji na platformy Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
