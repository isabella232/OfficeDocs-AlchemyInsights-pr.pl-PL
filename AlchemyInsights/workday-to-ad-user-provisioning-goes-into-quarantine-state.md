---
title: Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481881"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny

**Inicjowanie obsługi użytkowników w dni robocze u użytkowników usługi AD przechodzi do stanu kwarantanny i w u usługi AD nie są tworzona żadna użytkownicy**

Zadanie inicjowania obsługi użytkowników usługi AD w dzień roboczy przeszedł do stanu kwarantanny, a w dziennikach inspekcji są wyświetlane zdarzenia niepowodzenia eksportu z komunikatem o **błędzie: OperationsError-SvcErr: Wystąpił błąd operacji. Dla usługi katalogowej nie skonfigurowano żadnego odwołania przełożonego. Usługa katalogowa nie może więc wydawać poleceń** do obiektów spoza tego lasu. Ten błąd jest zazwyczaj wyświetlany, jeśli obiekt OU kontenera usługi Active Directory nie został poprawnie skonfigurowany lub występują problemy z mapowaniem wyrażeń używanym dla elementu **parentDistinguishedName.**

Sprawdź, czy parametr Default OU for New Users (Domyślna wersja systemu operacyjnego dla **nowych użytkowników)** nie zawiera literówek. Upewnij się, że określona grupa OU już istnieje w ad. Jeśli używasz wartości **parentDistinguishedName** podczas mapowania atrybutów, upewnij się, że zawsze jest szacowana jako znany kontener w domenie usługi AD. Sprawdź zdarzenie Eksportowanie w dziennikach inspekcji, aby wyświetlić wygenerowaną wartość.

Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego [dla automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

