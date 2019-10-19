---
title: Kod błędu 550 5.7.501 odmowa dostępu, wykryto nadużycie spamu
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36740151"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 odmowa dostępu, wykryto nadużycia spamu

Zazwyczaj ten komunikat występuje, gdy użytkownicy wysyłać wiadomości e-mail z adresów IP przy użyciu Initial *. onmicrosoft.com* domeny, która jest przypisana do nowych dzierżawców w pakiecie Office 365. Najprostszym sposobem rozwiązania tego problemu jest:

1. [Dodaj domenę do dzierżawy](https://docs.microsoft.com//office365/admin/setup/add-domain).

2. [Zmień podstawowy adres e-mail użytkowników](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) na nową domenę niestandardową, którą właśnie dodałeś.
