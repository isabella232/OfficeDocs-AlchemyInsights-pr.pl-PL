---
title: Instalator DKIM w usłudze Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765297"
---
# <a name="setup-dkim-in-office-365"></a>Instalator DKIM w usłudze Office 365

Kompletne instrukcje dotyczące konfigurowania DKIM dla domen niestandardowych w usłudze Office 365 są [tutaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Dla **każdej** domeny niestandardowe należy utworzyć **dwa** rekordy DKIM CNAME w usłudze hostingowej DNS domeny (zazwyczaj rejestratora domen). Na przykład contoso.com i fourthcoffee.com wymagają cztery rekordy DKIM CNAME: dwa dla domeny contoso.com i dwa dla fourthcoffee.com.

   Rekordy DKIM CNAME dla **każdej** domeny niestandardowe użyć następujących formatów:

   - **Nazwa hosta**:`selector1._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nazwa hosta**:`selector2._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> tekst z lewej strony jest `.mail.protection.outlook.com` w dostosowanych rekord MX dla domeny niestandardowej (na przykład `contoso-com` dla domeny contoso.com). \<InitialDomain\> jest domena używana podczas rejestrowania się w usłudze Office 365 (na przykład contoso.onmicrosoft.com).

2. Po utworzeniu rekordy CNAME dla domen niestandardowych, należy wykonać następujące instrukcje:

   . [Zaloguj się do usługi Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) , potrzebne do tego będzie Twoje konto służbowe.

   b. Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.

   c. W lewym dolnym nawigacji rozwiń **Admin** i wybierz **Exchange**.

   d. Przejdź do **ochrony** > **DKIM**.

   e. Wybierz domenę, a następnie wybierz polecenie **Włącz** **znak**wiadomości dla tej domeny z podpisami DKIM. Powtórz ten krok dla każdej domeny niestandardowej.
