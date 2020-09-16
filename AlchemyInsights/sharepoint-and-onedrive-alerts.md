---
title: Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727253"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Opóźnienia w otrzymywaniu alertów programu SharePoint i usługi OneDrive

- Najpierw sprawdź folder wiadomości-śmieci lub spam w wiadomości e-mail.
- Jeśli **wszystkie alerty z wielu plików lub bibliotek są opóźnione**, odwiedź [pulpit nawigacyjny kondycja usługi](https://portal.office.com/adminportal/home?ref=/servicehealth) , aby sprawdzić, jakie klasyfikatory/incydenty mogą wystąpić w programie SharePoint lub programie Exchange. Problem może dotyczyć funkcji alertów programu SharePoint lub opóźnień w wiadomościach e-mail za pośrednictwem programu Exchange. Sprawdź także, czy jest dostarczany inny adres e-mail — Jeśli nie, prawdopodobnie problem dotyczy opóźnień programu Exchange.
- Jeśli **pojedynczy alert z określonego pliku lub biblioteki nie jest dostarczany**, spróbuj go usunąć i utworzyć ponownie. Zobacz [Zarządzanie, wyświetlanie lub usuwanie alertów programu SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) w celu ponownego utworzenia alertu.

> [!NOTE]
> - Nie można wysyłać alertów do grupy dystrybucyjnej. Obsługiwane są tylko grupy zabezpieczeń i usługi Office 365.
> - Nie można dostosowywać szablonów wiadomości e-mail dotyczących alertów. Aby uzyskać te zmiany, należy użyć przepływu pracy Microsoft Flow lub SharePoint Designer.
