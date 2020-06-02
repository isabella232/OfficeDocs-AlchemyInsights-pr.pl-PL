---
title: Kod błędu 550 5.7.501 Odmowa dostępu, wykryto nadużycie spamu
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 9fd4f14798f27e7bf93daceb3620aff9b7f9e8ed
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506820"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Odmowa dostępu, wykryto nadużycie spamu

Zazwyczaj ten komunikat występuje, gdy użytkownicy wysyłają wiadomości e-mail z adresów IP przy użyciu początkowej domeny *.onmicrosoft.com,* która jest przypisana do nowych dzierżaw w usłudze Microsoft 365. Najprostszym sposobem rozwiązania tego problemu jest:

1. [Dodaj domenę do dzierżawy](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Zmień podstawowy adres e-mail użytkowników](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na nową domenę niestandardową, którą właśnie dodałeś.
