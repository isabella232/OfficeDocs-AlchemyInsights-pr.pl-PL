---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312697"
---
# <a name="alert-policies"></a>Zasady alertów

Microsoft 365 domyślne zasady [alertów](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) wyzwalają alerty dla organizacji z subskrypcją usługi Microsoft 365 Enterprise lub Microsoft 365 government E1/G1, E3/G3 lub E5/G5. Dlatego administratorzy mogą otrzymywać powiadomienia e-mail z alertami wysłane przez firmę Office365Alerts@microsoft.com z wierszem tematu, takim jak "Alert o niskim poziomie ważności: nazwa zasad *alertu*". Powiadomienia alertów są wysyłane w przypadku wyzwolenia alertów dotyczących typowych działań, na przykład gdy użytkownicy:

- Tworzenie reguł skrzynki odbiorczej do przesyłania dalej wiadomości e-mail.
- Przypisywanie uprawnień do skrzynki pocztowej.
- Udostępnianie lub usuwanie dużej liczby plików w SharePoint udostępniania plików.
- Tworzenie wyszukiwań zbierania elektronicznych materiałów dowodowych i eksportowanie wyników wyszukiwania.

Aby przejrzeć alert i działać w jego przypadku:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **alertów.** Aby przejść bezpośrednio do strony **Alerty,** użyj <https://compliance.microsoft.com/compliancealerts> .
   - W portalu Microsoft 365 Defender przejdź do tematu Alerty o <https://security.microsoft.com> **&** \> **zdarzeniach.** Aby przejść bezpośrednio do strony **Alerty,** użyj <https://security.microsoft.com/alerts> .
2. Kliknij alert, aby wyświetlić stronę wysuwu z informacjami o tym alertie.

Możesz podjąć działania dotyczące alertu, takie jak usunięcie [podejrzanej reguły skrzynki odbiorczej.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Możesz też po prostu zamknąć alert, klikając pozycję Rozwiąż **na** wysuwanym stronie alertu.

Aby uzyskać więcej informacji na temat konfigurowania zasad alertów i zarządzania nimi, [zobacz ten artykuł.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Ważne:** Powiadomienia e-mail od firmy Microsoft nigdy nie będą prosić o:

- Podaj hasło
- Weryfikowanie szczegółów zabezpieczeń konta
- Ponowne uwierzytelnienie siebie

Jeśli otrzymasz wiadomość e-mail z tego typu żądaniami, nie została ona wysłana przez firmę Microsoft i powinna być uznawana za próbę wyłudzenia informacji. Jeśli otrzymasz wiadomość z tego typu żądaniami, zgłoś tę wiadomość [firmie Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)
