---
title: Identyfikator aktywności reguły skrzynki odbiorczej w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779061"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identyfikator aktywności reguły skrzynki odbiorczej w dziennikach inspekcji

Aby wyświetlić zdarzenia reguły skrzynki odbiorczej (tworzenie, modyfikowanie i usuwanie reguł skrzynek odbiorczych), można użyć funkcji wyszukiwania dziennika inspekcji w centrum zgodności usługi Microsoft 365 Security &.

1. Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).

2. Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.

3. Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia** .

4. W obszarze **działania dotyczące skrzynek pocztowych programu Exchange**Sprawdź, czy w polu **działania** jest ustawiona wartość **Nowy — InboxRule tworzenie/modyfikowanie/Włączanie/wyłączanie reguły skrzynki odbiorczej**.

5. Kliknij przycisk **Wyszukaj**.

W wynikach wybierz rekord inspekcji. W menu wysuwanym Szczegóły kliknij pozycję **więcej informacji**. Informacje na temat ustawień reguły skrzynki odbiorczej są wyświetlane w polu **Parametry** .

Aby uzyskać więcej informacji, zobacz [Określanie, czy użytkownik utworzył regułę skrzynki odbiorczej](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
