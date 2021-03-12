---
title: DLP nie działa zgodnie z oczekiwaniami
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707820"
---
# <a name="dlp-not-working-as-expected"></a>DLP nie działa zgodnie z oczekiwaniami

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurowanie zasad DLP**

Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention) w** usłudze Office 365 nie działa zgodnie z oczekiwaniami? Jeśli tak, upewnij się, że zasady **DLP** zostały poprawnie skonfigurowane i że dane zawierają szukane zasady **DLP** podczas ich oceny.
  
Zasady DLP umożliwiają identyfikowanie i ochronę informacji poufnych w organizacji. Aby skonfigurować zasady DLP, skorzystaj z informacji w tym [miejscu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Jakie zasady ochrony przed zasadami ochrony przed zasadami DLP należy szukać**
  
Podczas korzystania **z** wbudowanych typów informacji poufnych w centrach zabezpieczeń i zgodności zasady DLP szukają określonych wzorców i elementów podczas wykrywania tych typów poufnych.
  
- **Wbudowane typy informacji poufnych**

    Aby uzyskać informacje o wbudowanych typach poufnych oraz o tym, co wyszukuje zasady DLP podczas wykrywania typu poufnego, zobacz: Czego szukają typy [informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Niestandardowe typy informacji poufnych**

    Jeśli próbujesz utworzyć niestandardowe typy informacji poufnych, skorzystaj z następującego artykułu, aby uzyskać informacje na temat tworzenia niestandardowego typu poufnego: Tworzenie niestandardowego typu informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testowanie zasad DLP**

Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu informacji poufnych, użyj opcji **Typ** testu w obszarze **Klasyfikacje** typów informacji  >  **poufnych.** Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raporty**
  
- Uzyskiwanie szczegółowych informacji o danych poufnych za pomocą [raportów DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
