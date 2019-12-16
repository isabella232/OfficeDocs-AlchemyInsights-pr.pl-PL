---
title: Powiadomienia alertów programu SharePoint nie są dostarczane
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047077"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Powiadomienia alertów programu SharePoint nie są dostarczane

Proszę sprawdzić folder wiadomości-śmieci w wiadomości e-mail, ponieważ czasami alerty mogą tam iść.

Określić, czy **wszystkie alerty nie są dostarczane** lub jeśli **pojedynczy alert** z określonego pliku lub biblioteki nie jest dostarczany.

- **Poszczególne alerty nie są dostarczane**: Jeśli pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony, można spróbować usunąć i odtworzyć go. Zobacz [Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint,](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) aby odtworzyć alert.
- **Wszystkie alerty nie są dostarczane**: Jeśli wszystkie alerty z wielu plików lub bibliotek nie są dostarczane, odwiedź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange. Problem może być z funkcji alertu programu SharePoint lub opóźnienia w wiadomościach e-mail za pośrednictwem programu Exchange. Ważne będzie również, aby pamiętać, czy inne wiadomości e-mail są dostarczane, a jeśli nie, problem jest prawdopodobne z opóźnień Exchange.

FAQ na temat alertów:

- Nie jest możliwe wysyłanie alertów do grupy dystrybucyjnej, obsługiwane są tylko grupy zabezpieczeń i 365.
- Nie można dostosować szablony wiadomości e-mail alertu; należy użyć przepływu pracy programu Microsoft FLOW lub SharePoint Designer do osiągnięcia tych.

Więcej informacji:

- **Ustawienia alertów**: Aby uzyskać więcej informacji na temat konfigurowania alertów, zobacz [Tworzenie alertu, aby otrzymywać powiadomienia, gdy plik lub folder zmieni się w programie SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Rozwiązywanie problemów z alertami**: Aby uzyskać więcej informacji na temat rozwiązywania problemów z alertami, zobacz [Użytkownicy nie otrzymują powiadomienia alertów online programu SharePoint](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Zaawansowane zasady alertów zgodności**z programem 365: Aby uzyskać więcej informacji na temat konfigurowania tych alertów, zobacz [zasady alertów zgodności](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **Dzienniki inspekcji programu SharePoint i OneDrive**: Aby uzyskać więcej informacji dotyczących sposobu pobierania tych zdarzeń, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Alerty wysyłane przez zaawansowaną ochronę przed zagrożeniami**: zobacz [ATP dla programu SharePoint i OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Alerty wysyłane przez zasady zapobiegania utracie danych**: zobacz [powiadomienia E-mail dotyczące zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Tematy pokrewne

Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?

- [Utwórz przepływ](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint i przepływu](https://flow.microsoft.com//blog/sharepoint-and-flow/)
