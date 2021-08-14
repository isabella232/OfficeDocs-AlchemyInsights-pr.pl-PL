---
title: Reguła DLP dla nie działa dla numeru konta bankowego w USA
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005028"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemy z DLP dotyczące numerów kont bankowych w USA

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP dotyczące numerów kont bankowych w USA**

Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention)** nie działa w przypadku zawartości zawierającej numer konta bankowego w USA podczas korzystania z typu informacji poufnych związanych z zapobieganiem utracie danych w U365?  Jeśli tak, upewnij się, że zawartość zawiera niezbędne informacje na potrzeby oceny zasad DLP.
  
Na przykład w  przypadku zasad numeru konta bankowego w Usa skonfigurowanych z poziomem ufności 85% są obliczane następujące i należy je wykrywać, aby reguła uruchamiała:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cyfr

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** od 8 do 17 kolejnych cyfr.

- **[Sumy kontrolne:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zasady DLP mają 75% pewności, że wykrywane są tego typu informacje poufne, jeśli w odległości 300 znaków:

  - Wyrażenie regularne Regex_usa_bank_account_number umożliwia znalezienie zawartości, która jest taka, jak wzorzec

  - Zostanie znalezione słowo kluczowe Keyword_usa_Bank_Account.

    Na przykład wyzwoliłyby  się zasady numeru konta bankowego w USA w następujący sposób: Sprawdzanie konta 78344011

Aby uzyskać więcej informacji na  temat tego, co jest wymagane, aby wykrywany przez Twoją zawartość numer konta bankowego w USA był wykrywany, zobacz następującą sekcję w tym artykule: Co typ informacji poufnych ma szukać w sekcji Numer konta [bankowego](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) w USA
  
Informacje wymagane dla innych typów można znaleźć w następującym artykule, w którym podano informacje o innych [typach:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Typy informacji poufnych
  