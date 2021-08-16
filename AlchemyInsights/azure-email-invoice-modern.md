---
title: Nowoczesne fakturowanie poczty e-mail platformy Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082844"
---
# <a name="email-invoicing-in-azure"></a>Fakturowanie poczty e-mail na platformie Azure

Aby zaktualizować preferencje dotyczące faktur e-mail, musisz mieć rolę właściciela lub współautora w profilu rozliczeniowym lub na jego koncie rozliczeniowym. Po wybraniu zgody wszyscy użytkownicy z rolami właściciela, współautora, czytelników i menedżera faktur w profilu rozliczeniowym otrzymają fakturę w wiadomości e-mail.

1. Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)
2. Szukaj w pozycji **Zarządzanie kosztami + rozliczenia**.
3. Wybierz **pozycję Faktury** z lewej strony, a następnie wybierz pozycję Wyślij fakturę pocztą e-mail u góry strony. 
4. Jeśli masz wiele profilów rozliczeniowych, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Wybierz opcję**.

5. Wybierz **pozycję Aktualizuj**.
6. Jeśli masz wiele profilów rozliczeniowych, wybierz profil rozliczeniowy, a następnie wybierz pozycję **Wybierz opcję**.

Możesz dać innym osobom dostęp do wyświetlania, pobierania i opłacania faktur, przypisując im rolę menedżera faktur dla profilu rozliczeniowego MCA lub MPA. Jeśli w wiadomości e-mail wybrałeś(-asz) fakturę, użytkownicy również otrzymają faktury w wiadomości e-mail.

1. Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/)
2. Szukaj w pozycji **Zarządzanie kosztami + rozliczenia**.
3. Wybierz **pozycję Profile rozliczeniowe** z lewej strony. Z listy profile rozliczeniowe wybierz profil rozliczeniowy, do którego chcesz przypisać rolę menedżera faktur.
4. Wybierz **pozycję Kontrola dostępu (IAM)** z lewej strony, a następnie wybierz pozycję **Dodaj** u góry strony.

Z listy rozwijanej Rola wybierz pozycję **Menedżer faktur**. Wprowadź adres e-mail użytkownika, który ma udzielić dostępu. Wybierz **pozycję Zapisz,** aby przypisać rolę.
