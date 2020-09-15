---
title: Układ DLP nie działa zgodnie z oczekiwaniami
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679703"
---
# <a name="dlp-not-working-as-expected"></a>Układ DLP nie działa zgodnie z oczekiwaniami

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurowanie DLP**

Czy problemy z **Zapobieganie utracie danych (DLP)** w pakiecie Office 365 nie działają zgodnie z oczekiwaniami? Jeśli tak, upewnij się, że **zasady DLP** są poprawnie skonfigurowane i że dane zawierają **zasady DLP** , które są używane podczas szacowania.
  
Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji. Aby skonfigurować zasady DLP, Skorzystaj z informacji w [tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Jakie zasady DLP wyglądają**
  
Gdy korzystasz z **wbudowanych typów informacji poufnych** w centrach zabezpieczeń i zgodności, zasady DLP szukają określonych wzorców i elementów podczas wykrywania tych wrażliwych typów.
  
- **Wbudowane typy informacji poufnych**

    Aby uzyskać informacje na temat wbudowanych typów poufnych oraz zasad DLP, które wyszukują podczas wykrywania typu poufnego, zobacz: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Niestandardowe typy informacji poufnych**

    Jeśli próbujesz utworzyć niestandardowe typy informacji poufnych, Skorzystaj z następującego artykułu, aby uzyskać informacje na temat tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testowanie zasad DLP**

Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu informacji poufnych, użyj opcji **typ testu** w obszarze **klasyfikacje**  >  **informacje wrażliwe**. Aby uzyskać więcej informacji, zobacz [testowanie typów niestandardowych informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Raporty**
  
- Uzyskiwanie ważnych danych w celu uwzględnienia [raportów DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Szczegółowe informacje o zdarzeniu można znaleźć w [raporcie dotyczącym incydentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
