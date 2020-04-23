---
title: Opóźnienia w odbieraniu alertów w programie SharePoint i OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742011"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Opóźnienia w odbieraniu alertów w programie SharePoint i OneDrive

- Najpierw sprawdź folder Wiadomości-śmieci lub Spam w wiadomości e-mail.
- Jeśli **wszystkie alerty z wielu plików lub bibliotek są opóźnione,** odwiedź [pulpit nawigacyjny kondycji usługi,](https://portal.office.com/adminportal/home?ref=/servicehealth) aby sprawdzić, czy nie ma żadnych porad/incydentów, które mogą występować w programie SharePoint lub Exchange. Problem może dotyczyć funkcji alertu programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange. Zwróć również uwagę, czy inna wiadomość e-mail jest dostarczana — jeśli nie, problem jest prawdopodobnie opóźniany w programie Exchange.
- Jeśli **pojedynczy alert z określonego pliku lub biblioteki nie zostanie dostarczony,** spróbuj go usunąć i ponownie utworzyć. Aby odtworzyć [alert, zobacz Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint.](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)

> [!NOTE]
> - Alertów nie można wysyłać do grupy dystrybucyjnej. Obsługiwane są tylko grupy zabezpieczeń i O365.
> - Nie można dostosować szablonów alertów wiadomości e-mail. Aby je osiągnąć, należy użyć usługi Microsoft Flow lub SharePoint Designer Workflow.
