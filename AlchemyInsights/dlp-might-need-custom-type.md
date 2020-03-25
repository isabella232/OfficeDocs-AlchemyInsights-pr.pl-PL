---
title: DLP może wymagać typu niestandardowego
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932668"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP może wymagać typu niestandardowego

**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle. Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych. W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.

W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia. Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach. Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.

**DLP może wymagać niestandardowego typu informacji**

Za pomocą zasad zapobiegania utracie danych (DLP) można identyfikować i chronić poufne dane w organizacji. W niektórych scenariuszach może być konieczne utworzenie własnego **niestandardowego** typu poufnych informacji w celu ochrony danych organizacji.

Na przykład organizacja może wymagać identyfikowania i ochrony identyfikatorów pracowników lub innych danych w formacie specyficznym dla organizacji. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.
  
 **Dostosowywanie wbudowanego typu poufnych informacji**
  
Jeśli wbudowany typ poufnych informacji odpowiadałby Twoim potrzebom za pomocą zaledwie kilku poprawek, możesz [dostosować wbudowany typ poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) Możesz na przykład dodać lub usunąć słowa kluczowe lub dodać lub usunąć dowody potwierdzające, takie jak data lub adres.
  
 **Tworzenie niestandardowego typu poufnych informacji**
  
Jeśli jednak musisz zidentyfikować i chronić zupełnie inny typ poufnych informacji, możesz [utworzyć niestandardowy typ poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika Centrum zgodności & zabezpieczeń.
  
**Tworzenie niestandardowego typu poufnych informacji w programie PowerShell centrum zabezpieczeń & Compliance Center**

Jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, można [utworzyć niestandardowy typ poufnych informacji w programie Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Zaczynając od pliku XML, można użyć każdej dostępnej opcji.
