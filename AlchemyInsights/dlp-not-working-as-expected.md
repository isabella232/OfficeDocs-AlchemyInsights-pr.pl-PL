---
title: DLP nie działa zgodnie z oczekiwaniami
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507488"
---
# <a name="dlp-not-working-as-expected"></a>DLP nie działa zgodnie z oczekiwaniami

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurowanie DLP**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami? Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawiera to, czego szukają **zasady DLP** podczas oceny.
  
Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji. Aby skonfigurować zasady DLP, użyj tych informacji [w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Czego szukają zasady DLP**
  
Podczas korzystania z **wbudowanych typów informacji poufnych** w centrach zabezpieczeń i zgodności zasady DLP wyszukują określone wzorce i elementy podczas wykrywania tych typów poufnych.
  
- **Wbudowane typy poufnych informacji**

    Aby uzyskać informacje na temat wbudowanych typów poufnych i tego, czego szukają zasady DLP podczas wykrywania typu poufnego, zobacz: [Czego szukają typy poufnych informacji.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Niestandardowe typy poufnych informacji**

    Jeśli próbujesz utworzyć niestandardowe typy poufnych informacji, użyj następującego artykułu, aby uzyskać informacje dotyczące tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testowanie zasad DLP**

Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu poufnych informacji, użyj opcji **Typ testu** w obszarze **Classifications**  >  **Typy informacji poufne**klasyfikacji . Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Raporty**
  
- Uzyskaj szczegółowe informacje o poufnych danych dzięki [raportom DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
