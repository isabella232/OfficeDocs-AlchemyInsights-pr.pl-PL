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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324000"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rozwiązywanie typowych problemów z formatowaniem rekordów DKIM

Większość problemów z konfigurowaniem DKIM jest związanych z niepoprawnymi rekordami DNS.

Aby rozwiązać problemy z konfigurowaniem usługi DKIM, upewnij się, że rekord CNAME DKIM **(a** nie rekord TXT) został prawidłowo sformatowany. Aby uzyskać więcej informacji, zobacz Co należy zrobić, aby ręcznie skonfigurować [DKIM w programie Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jeśli potrzebujesz pomocy dotyczącej ogólnych rekordów DNS, zobacz Tworzenie rekordów DNS dla usługi w witrynie [Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Uwaga:** Po utworzeniu lub zaktualizowaniu rekordów DNS DKIM w usłudze hostingu DNS domeny musisz zaczekać na propagację rekordów DNS.
