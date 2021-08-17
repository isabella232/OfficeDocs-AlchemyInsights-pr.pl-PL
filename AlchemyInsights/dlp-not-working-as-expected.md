---
title: Działanie zasad DLP nie działa zgodnie z oczekiwaniami
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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079712"
---
# <a name="dlp-not-working-as-expected"></a>Działanie zasad DLP nie działa zgodnie z oczekiwaniami

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurowanie zasad DLP**

Czy masz problemy z zapobieganiem **utracie danych (DLP, Data Loss Prevention)** w programie Office 365 nie działa zgodnie z oczekiwaniami? Jeśli tak, upewnij się, że zasady **DLP** są skonfigurowane poprawnie i że dane zawierają szukane zasady **DLP** podczas ich oceny.
  
Zasady DLP umożliwiają identyfikowanie i ochronę informacji poufnych w organizacji. Aby skonfigurować zasady DLP, skorzystaj z informacji w tym [miejscu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Czego szukać w zasadach ochrony przed zasadami DLP**
  
W przypadku korzystania **z wbudowanych** typów informacji poufnych w centrach zabezpieczeń i zgodności zasady DLP szukają określonych wzorców i elementów podczas wykrywania tych typów poufnych.
  
- **Wbudowane typy informacji poufnych**

    Aby uzyskać informacje o wbudowanych typach poufnych oraz o tym, co zasady DLP wyszukuje podczas wykrywania typu poufnego, zobacz: Czego szukać w przypadku typów informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Niestandardowe typy informacji poufnych**

    Jeśli próbujesz utworzyć niestandardowe typy informacji poufnych, skorzystaj z następującego artykułu, aby uzyskać informacje na temat tworzenia niestandardowego typu poufnego: Tworzenie niestandardowego typu informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testowanie zasad DLP**

Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu informacji poufnych, użyj opcji **Typ testu** w obszarze **Klasyfikacje typów** informacji  >  **poufnych.** Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raporty**
  
- Uzyskiwanie szczegółowych informacji o danych dzięki raportom [DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
