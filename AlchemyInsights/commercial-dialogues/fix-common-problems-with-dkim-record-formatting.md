---
title: Rozwiązywanie typowych problemów z formatowaniem rekordów DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930071"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rozwiązywanie typowych problemów z formatowaniem rekordów DKIM

Większość problemów z konfigurowaniem DKIM jest związanych z niepoprawnymi rekordami DNS.

Aby rozwiązać problemy z konfigurowaniem usługi DKIM, upewnij się, że rekord CNAME DKIM **(a** nie rekord TXT) został prawidłowo sformatowany. Aby uzyskać więcej informacji, zobacz Co należy zrobić, aby ręcznie skonfigurować [DKIM w programie Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jeśli potrzebujesz pomocy dotyczącej ogólnych rekordów DNS, zobacz Tworzenie rekordów DNS dla usługi [w](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)witrynie Office 365.

> [!NOTE]
> Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS domeny musisz zaczekać na propagację rekordów DNS.
