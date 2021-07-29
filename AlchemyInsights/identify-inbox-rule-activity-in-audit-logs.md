---
title: Identyfikowanie działań reguł skrzynki odbiorczej w dziennikach inspekcji
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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630187"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identyfikowanie działań reguł skrzynki odbiorczej w dziennikach inspekcji

Zdarzenia reguł skrzynki odbiorczej (tworzenie, modyfikowanie i usuwanie reguł skrzynki odbiorczej) Microsoft 365 przy użyciu funkcji przeszukiwania dziennika inspekcji w Centrum & zabezpieczeń i zgodności.

1. Zaloguj się do [centrum Microsoft 365 zgodności.](https://protection.office.com/)

2. Przejdź do **strony Przeszukiwanie**  >  **dziennika inspekcji wyszukiwania.**

3. Zaznacz zakres dat w **polach Data rozpoczęcia** **i Data zakończenia.**

4. W **Exchange skrzynki** pocztowej sprawdź, czy pole Działania ma ustawioną wartość Nowa skrzynka odbiorczaZamówienie  **Create/modify/enable/disable/inbox rule.**

5. Kliknij **przycisk Wyszukaj**.

W wynikach wybierz rekord inspekcji. W wysuwanych szczegółach kliknij pozycję **Więcej informacji**. Informacje o ustawieniach reguły skrzynki odbiorczej są wyświetlane w polu **Parametry.**

Aby uzyskać więcej informacji, zobacz [Ustalanie, czy użytkownik utworzył regułę skrzynki odbiorczej.](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
