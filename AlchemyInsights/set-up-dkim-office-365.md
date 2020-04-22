---
title: Konfiguracja DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645682"
---
# <a name="setup-dkim"></a>Konfiguracja DKIM

Pełne instrukcje konfigurowania DKIM dla domen niestandardowych w usłudze Microsoft 365 znajdują [się tutaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Dla **każdej** domeny niestandardowej należy utworzyć **dwa** rekordy CNAME DKIM w usłudze hostingu DNS domeny (zazwyczaj rejestratora domen). Na przykład contoso.com i fourthcoffee.com wymagać czterech rekordów CNAME DKIM: dwóch dla contoso.com i dwóch dla fourthcoffee.com.

   Rekordy CNAME DKIM dla **każdej** domeny niestandardowej używają następujących formatów:

   - **Nazwa hosta**:`selector1._domainkey.<CustomDomain>`

     **Wskazuje na adres lub wartość:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nazwa hosta**:`selector2._domainkey.<CustomDomain>`

     **Wskazuje na adres lub wartość:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> to tekst znajdujący `.mail.protection.outlook.com` się po lewej stronie w dostosowanym rekordzie MX dla domeny niestandardowej (na przykład `contoso-com` dla domeny contoso.com). \<InitialDomain\> to domena używana podczas konfigurowania usługi Microsoft 365 (na przykład contoso.onmicrosoft.com).

2. Po utworzeniu rekordów CNAME dla domen niestandardowych wykonaj następujące instrukcje:

   A. [zaloguj się do usługi Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) za pomocą konta służbowego.

   B. Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.

   C. W lewym dolnym lewym przycisku nawigacji rozwiń pozycję **Administrator** i wybierz pozycję **Exchange**.

   D. Przejdź do **ochrony** > **DKIM**.

   E. Wybierz domenę, a następnie wybierz pozycję **Włącz** dla **sygnatariuszy wiadomości dla tej domeny z podpisami DKIM**. Powtórz ten krok dla każdej domeny niestandardowej.
