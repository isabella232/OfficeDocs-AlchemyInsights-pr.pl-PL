---
title: Konfigurowanie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108566"
---
# <a name="setup-dkim"></a>Konfigurowanie DKIM

Tutaj znajdziesz pełne instrukcje dotyczące konfigurowania usługi DKIM dla domen Microsoft 365 [niestandardowych.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Dla **każdej** domeny niestandardowej musisz utworzyć dwa rekordy **DKIM** CNAME w usłudze hostingu DNS swojej domeny (zwykle jest to rejestrator domeny). Na przykład contoso.com i fourthcoffee.com czterech rekordów DKIM CNAME: dwa dla contoso.com i dwa dla fourthcoffee.com.

   Rekordy CNAME DKIM dla **każdej domeny** niestandardowej używają następujących formatów:

   - **Nazwa hosta:**`selector1._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (Czas wygaśnięcia):** 3600

   - **Nazwa hosta:**`selector2._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (Czas wygaśnięcia):** 3600

   \<DomainGUID\> to tekst po lewej stronie niestandardowego rekordu MX domeny niestandardowej (na przykład dla domeny `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>jest domeną używaną podczas rejestracji w u Microsoft 365 (na przykład contoso.onmicrosoft.com).

2. Po utworzeniu rekordów CNAME dla domen niestandardowych wykonaj następujące instrukcje:

   a. [, aby Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) za pomocą konta służbowego.

   b. Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.

   c. W lewym dolnym rogu nawigacji rozwiń pozycję **Administrator** i wybierz pozycję **Exchange.**

   d. Przejdź do **ochrony**  >  **DKIM.**

   e. Wybierz domenę, a następnie wybierz **pozycję Włącz** dla opcji **Podpisz wiadomości dla tej domeny przy użyciu podpisów DKIM.** Powtórz ten krok dla każdej domeny niestandardowej.
