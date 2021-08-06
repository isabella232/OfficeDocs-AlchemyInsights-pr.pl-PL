---
title: W dni robocze inicjowanie obsługi użytkowników usługi AD przechodzi w stan kwarantanny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036502"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>W dni robocze inicjowanie obsługi użytkowników usługi AD przechodzi w stan kwarantanny

**Inicjowanie obsługi użytkowników w dni robocze do usługi AD przechodzi w stan kwarantanny i w u nich nie są tworzona żadna użytkownicy**

Zadanie inicjowania obsługi użytkowników w dni robocze dla użytkowników usługi AD przeszło do stanu kwarantanny, a w dziennikach inspekcji są wyświetlane zdarzenia niepowodzenia eksportu z komunikatem o błędzie **Błąd: OperationsError-SvcErr: Wystąpił błąd operacji. Dla usługi katalogowej nie skonfigurowano żadnego przełożonego. Usługa katalogowa nie może więc wydawać poleceń do obiektów spoza tego lasu.** Ten błąd jest zazwyczaj wyświetlany, jeśli obiekt OU kontenera usługi Active Directory nie został prawidłowo skonfigurowany lub występują problemy z mapowaniem wyrażeń używanym dla elementu **parentDistinguishedName.**

Sprawdź, czy parametr Default OU for **New Users (Nowi użytkownicy)** nie zawiera literówek. Upewnij się, że określona grupa OU już istnieje w u ad. Jeśli używasz wartości **parentDistinguishedName** w mapowaniu atrybutów, upewnij się, że zawsze jest szacowana jako znany kontener w domenie usługi AD. Sprawdź zdarzenie Export (Eksportuj) w dziennikach inspekcji, aby zobaczyć wygenerowaną wartość.

Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego dla [automatycznego inicjowania obsługi użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

