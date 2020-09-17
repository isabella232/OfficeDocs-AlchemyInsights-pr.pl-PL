---
title: Konfiguracja DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808717"
---
# <a name="setup-dkim"></a>Konfiguracja DKIM

Pełne instrukcje dotyczące konfigurowania DKIM dla domen niestandardowych w programie Microsoft [365 są dostępne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. W przypadku **każdej** domeny niestandardowej trzeba utworzyć **dwa** DKIM rekordy CNAME w usłudze hostingu DNS domeny (zazwyczaj rejestrator domen). Na przykład contoso.com i fourthcoffee.com wymaga czterech DKIM rekordów CNAME: dwóch dla contoso.com i dwóch dla fourthcoffee.com.

   W rekordach CNAME DKIM dla **każdej** domeny niestandardowej zastosowano następujące formaty:

   - **Nazwa hosta**: `selector1._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **Czas wygaśnięcia**: 3600

   - **Nazwa hosta**: `selector2._domainkey.<CustomDomain>`

     **Wskazuje adres lub wartość**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **Czas wygaśnięcia**: 3600

   \<DomainGUID\> jest tekstem po lewej stronie `.mail.protection.outlook.com` dostosowanego rekordu MX dla domeny niestandardowej (na przykład `contoso-com` dla contoso.com domeny). \<InitialDomain\> jest domeną używaną podczas tworzenia konta w usłudze Microsoft 365 (na przykład contoso.onmicrosoft.com).

2. Po utworzeniu rekordów CNAME dla domen niestandardowych wykonaj następujące instrukcje:

   a. [Zaloguj się do usługi Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) za pomocą konta służbowego lub szkolnego.

   b. Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.

   c. W lewym dolnym okienku nawigacji rozwiń pozycję **administrator** i wybierz pozycję **Exchange**.

   d. Przejdź na stronę **Ochrona**  >  **DKIM**.

   e. Wybierz domenę, a następnie wybierz pozycję **Włącz** dla **podpisywania wiadomości dla tej domeny z podpisami DKIM**. Powtórz ten krok dla każdej domeny niestandardowej.
