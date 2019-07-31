---
title: DLP nie działa zgodnie z oczekiwaniami
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941078"
---
# <a name="dlp-not-working-as-expected"></a>DLP nie działa zgodnie z oczekiwaniami

Czy masz problemy z **Zapobiegania utraty danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami? Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawierają jakie **zasady DLP** poszukuje podczas jest oceniana.
  
 **Definiowanie DLP**
  
Zasady DLP pozwala zidentyfikować i ochrony poufnych informacji w danej organizacji. Konfiguracja zasad DLP, należy użyć informacji [w tym polu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Jakie zasady DLP szukać**
  
Korzystając z **typów wbudowanych poufnych informacji** w Centrum Office 365 bezpieczeństwa i zgodności, zasad DLP szukać określonych wzorców i elementów podczas wykrywania tego typu wrażliwe.
  
- **Typy wbudowane poufnych informacji**

    Szczegółowe informacje o wbudowanych typów wrażliwych i co zasad DLP szuka podczas wykrywania typu wrażliwe,: [poszukaj jakie typy informacji poufnych](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Typy niestandardowe informacje poufne**

    Jeśli próbujesz utworzyć typy niestandardowe informacje poufne, użyj następującego artykułu informacji na temat tworzenia niestandardowego typu poufne: [Utwórz typ niestandardowy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testowanie zasad DLP**

Aby przetestować danych o typie wbudowane lub niestandardowe poufne informacje, należy użyć opcji **Typ testu** w obszarze **Klasyfikacje** > **typów poufnych informacji**. Aby uzyskać więcej informacji zobacz [Typy niestandardowe informacje poufne testu](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Raporty**
  
- Wyszukaj informacje poufne dane z [DLP raportów.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Zobacz szczegółowe informacje dotyczące zdarzeń [Incydentu raport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)z.
