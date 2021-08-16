---
title: Powiadomienia w usłudze Yammer
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
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097208"
---
# <a name="notifications-in-yammer"></a>Powiadomienia w usłudze Yammer

Aby poinformować Cię o nowej aktywności w odpowiednich konwersacjach, [usługa Yammer wysyła powiadomienia](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) za pośrednictwem poczty e-mail albo — jeśli używasz usługi Yammer na urządzeniu przenośnym — za pośrednictwem powiadomień wypychanych. Domyślnie usługa Yammer wysyła powiadomienia dla wielu typów aktywności w Twojej sieci. Użytkownicy mogą aktualizować swoje ustawienia poczty e-mail za pośrednictwem witryny internetowej usługi Yammer, a powiadomienia wypychane są konfigurowane za pośrednictwem aplikacji dla urządzeń przenośnych. 

Usługa Yammer dodała obsługę [interakcyjnych wiadomości e-mail w programie Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). W aplikacji Outlook w sieci Web niektóre wiadomości e-mail (kopie wiadomości) staną się interakcyjne. Przyszła aktualizacja spowoduje wprowadzenie tej funkcji do innych wersji programu Outlook.

**Typy powiadomień w usłudze Yammer**

- Wiadomości e-mail (aktualizacje z grupy, ktoś zaprasza Cię do grupy, otrzymujesz wiadomość w skrzynce odbiorczej itp.).
- Powiadomienia wypychane (wysyłane do urządzeń przenośnych, na których jest wzmianka o Tobie, odbierające wiadomości w skrzynce odbiorczej itp.).
- Klasyczne menu podręczne (gdy masz zainstalowaną aplikację klasyczną Yammer, wyświetli ona powiadomienia dla użytkowników o nazwie „wyskakujące” powiadomienia).
- Powiadomienia w kształcie dzwonka (wewnątrz witryny internetowej usługi Yammer użytkownicy zobaczą powiadomienia dla różnych zdarzeń. Te powiadomienia mogą nie zawsze mieć skojarzone konta e-mail ani powiadomienia wypychane).

Dostępne są bardziej [szczegółowe informacje na temat powiadomień](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Zarządzanie powiadomieniami**

Użytkownicy muszą zarządzać własnymi powiadomieniami. Informacje są dostępne w temacie dotyczącym [sposobu włączania i wyłączania powiadomień usługi Yammer dla poczty e-mail i urządzeń mobilnych](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratorzy nie mogą wyłączyć wszystkich powiadomień ani kontrolować powiadomień w imieniu użytkowników. Administratorzy mogą [kontrolować logo zawarte w wiadomościach e-mail oraz zdecydować, czy użytkownicy będą musieli potwierdzać wiadomości](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) opublikowane za pośrednictwem poczty e-mail.

**Powiadomienia e-mail wysyłane do wielu użytkowników w organizacji**

Czasami usługa Yammer będzie wysyłać pojedyncze powiadomienia e-mail, które będą odbierane przez znacznie większą liczbę użytkowników w organizacji niż można się było spodziewać. Dzieje się tak, gdy do usługi Yammer zostanie dodana lista dystrybucyjna lub inny typ adresu e-mail nienależącego do konkretnej osoby. Usługa Yammer nie wie we wszystkich przypadkach, czy adres e-mail należy do jednego użytkownika lub czy jest to adres e-mail, który spowoduje dostarczenie jednej wiadomości e-mail do wielu adresatów. W przypadku wystąpienia tego problemu należy podjąć akcję, aby [zawiesić (dezaktywować) nieprawidłowego użytkownika z tym adresem e-mail](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) w usłudze Yammer. 

W celu zmniejszenia prawdopodobieństwa wystąpienia tego problemu należy:

1. [Wymusić tożsamość usługi Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) dla usługi Yammer.
2. Zablokować wysyłanie przez nadawców zewnętrznych wiadomości e-mail do organizacji lub ograniczyć nadawców do zatwierdzonej listy.

Jeśli ten problem wystąpi:

1. Zidentyfikuj adresata wiadomości e-mail, który powinien być zgodny z użytkownikiem usługi Yammer. Na przykład all-in-sales@fabrikam.com to lista dystrybucyjna dla wszystkich sprzedawców. Na podstawie wiadomości e-mail usługi Yammer odebranych przez użytkowników będzie możliwa identyfikacja tej listy dystrybucyjnej.
2. Za pomocą funkcji [dezaktywacji (zawieszenia) w administracji sieci](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) można zawiesić użytkownika, który ma adres e-mail all-in-sales@fabrikam.com. Zawieszenie można cofnąć, więc jest to bezpieczniejsze od usunięcia. Usunięcie użytkownika nastąpi automatycznie po 90 dniach.
3. Opcjonalnie zapoznaj się z funkcją [Eksportuj użytkownika](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), aby zidentyfikować inne adresy e-mail, które nie odpowiadają użytkownikom i które powinny zostać zawieszone.
