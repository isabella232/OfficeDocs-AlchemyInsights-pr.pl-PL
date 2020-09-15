---
title: Reguła DLP dla numeru konta bankowego nie działa w Stanach Zjednoczonych
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679306"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemy dotyczące DLP w numerach kont bankowych Stanów Zjednoczonych

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy dotyczące DLP w numerach kont bankowych Stanów Zjednoczonych**

Czy problemy związane z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer konta bankowego w Stanach Zjednoczonych** w przypadku korzystania z informacji poufnych dotyczących DLP w usłudze Office 365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, co mają zasady DLP podczas szacowania.
  
Na przykład w przypadku zasad **numeru konta bankowego Stanów Zjednoczonych** skonfigurowanych z poziomem ufności równą 85% zostaną obliczone następujące obliczenia i trzeba je wykryć, aby reguła była wyzwalana:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cyfr

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 kolejnych cyfr.

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zasady DLP to 75% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:

  - Wyrażenie regularne Regex_usa_bank_account_number umożliwia Znajdowanie zawartości zgodnej ze wzorcem

  - Znaleziono słowo kluczowe from Keyword_usa_Bank_Account.

    Na przykład Poniższa przykładowa zasada **numeru konta bankowego Stanów Zjednoczonych** : sprawdzanie konta 78344011

Aby uzyskać więcej informacji na temat tego, co jest wymagane, aby **numer konta bankowego w Stanach Zjednoczonych** był wykrywany dla zawartości, zapoznaj się z poniższą sekcją w tym artykule: co to są [typy informacji wrażliwych na numer konta bankowego](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .
  
Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .
  