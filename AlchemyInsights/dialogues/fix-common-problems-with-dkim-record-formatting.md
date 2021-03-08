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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525650"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rozwiązywanie typowych problemów z formatowaniem rekordów DKIM

Większość problemów z konfigurowaniem DKIM jest związanych z niepoprawnymi rekordami DNS.

Aby rozwiązać problemy z konfigurowaniem DKIM, upewnij się, że rekord CNAME DKIM **(nie** rekord TXT) został prawidłowo sformatowany. Aby uzyskać więcej informacji, zobacz Co należy zrobić, aby ręcznie skonfigurować [DKIM w usłudze Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jeśli potrzebujesz pomocy dotyczącej ogólnych rekordów DNS, zobacz tworzenie rekordów DNS dla usługi [Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)u dowolnego dostawcy hostingu DNS.

> [!NOTE]
> Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS domeny musisz zaczekać na propagację rekordów DNS.
