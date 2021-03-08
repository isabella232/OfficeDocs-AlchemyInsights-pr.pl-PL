---
title: Konfigurowanie usługi DKIM przy użyciu domen niestandardowych
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525415"
---
# <a name="set-up-dkim-with-custom-domains"></a>Konfigurowanie usługi DKIM przy użyciu domen niestandardowych

Musisz opublikować dwa rekordy CNAME dla każdej domeny niestandardowej w systemie DNS. Aby to zrobić, użyj następującego formatu:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** to tekst po lewej stronie nazwy **.mail.protection.outlook.com** w dostosowanym rekordzie MX domeny niestandardowej (na przykład contoso-com dla domeny **contoso.com).** **InitialDomain** to domena używana podczas rejestracji w usłudze Office 365 (na przykład **contoso.onmicrosoft.com).**

Aby uzyskać więcej informacji na temat rekordów DNS, zobacz Tworzenie rekordów DNS dla usługi [Office 365 u](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)dowolnego dostawcy hostingu DNS.