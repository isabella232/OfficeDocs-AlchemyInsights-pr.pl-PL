---
title: Powiadomienia alertów programu SharePoint nie zostały dostarczone
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742057"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Powiadomienia alertów programu SharePoint nie zostały dostarczone

Sprawdź folder ŚMIECI w wiadomości e-mail, ponieważ czasami mogą tam trafić alerty.

Określ, czy **wszystkie alerty nie są dostarczane** lub jeśli pojedynczy **alert** z określonego pliku lub biblioteki nie jest dostarczany.

- **Poszczególne alerty nie są dostarczane:** Jeśli pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony, można spróbować go usunąć i ponownie utworzyć. Aby odtworzyć [alert, zobacz Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint.](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)
- **Wszystkie alerty nie są dostarczane:** Jeśli wszystkie alerty z wielu plików lub bibliotek nie są dostarczane, odwiedź [pulpit nawigacyjny kondycji usługi,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange. Problem może dotyczyć funkcji alertu programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange. Ważne będzie również, aby pamiętać, czy inna wiadomość e-mail jest dostarczana, a jeśli nie, problem jest prawdopodobnie związany z opóźnieniami programu Exchange.

Często zadawane pytania dotyczące alertów:

- Nie można wysyłać alertów do grupy dystrybucyjnej, obsługiwane są tylko grupy zabezpieczeń i usługi O365.
- Nie można dostosować szablonów alertów poczty e-mail; aby je osiągnąć, musisz użyć programu Microsoft FLOW lub SharePoint Designer Workflow.

Więcej informacji:

- **Konfiguracja alertów:** Aby uzyskać więcej informacji na temat konfigurowania alertów, zobacz [Tworzenie alertu, aby otrzymywać powiadomienia o zmianie pliku lub folderu w programie SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Rozwiązywanie problemów z alertami:** Aby uzyskać więcej informacji na temat alertów dotyczących rozwiązywania problemów, zobacz [Użytkownicy nie otrzymują powiadomień o alertach usługi SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Zaawansowane zasady alertów zgodności usługi O365**: Aby uzyskać więcej informacji na temat konfigurowania tych alertów, zobacz [Zasady alertów zgodności](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **Dzienniki inspekcji programu SharePoint i OneDrive**: Aby uzyskać więcej informacji na temat pobierania tych zdarzeń, zobacz [Wyszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Alerty wysyłane przez zaawansowaną ochronę przed zagrożeniami:** Zobacz [ATP dla programu SharePoint i OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Alerty wysyłane przez zasady zapobiegania utracie danych**: Zobacz [powiadomienia e-mail dla zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Tematy pokrewne

Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?

- [Utwórz przepływ](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [Program SharePoint i przepływ](https://flow.microsoft.com//blog/sharepoint-and-flow/)
