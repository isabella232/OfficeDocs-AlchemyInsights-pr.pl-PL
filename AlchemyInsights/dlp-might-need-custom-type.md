---
title: DLP może wymagać typu niestandardowego
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704499"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP może wymagać typu niestandardowego

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP może wymagać niestandardowego typu informacji**

Za pomocą zasad zapobiegania utracie danych (DLP) można identyfikować i chronić poufne dane w organizacji. W niektórych scenariuszach może być konieczne utworzenie własnego **niestandardowego** typu poufnych informacji w celu ochrony danych organizacji.

Na przykład organizacja może wymagać identyfikowania i ochrony identyfikatorów pracowników lub innych danych w formacie specyficznym dla organizacji. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.
  
 **Dostosowywanie wbudowanego typu poufnych informacji**
  
Jeśli wbudowany typ poufnych informacji odpowiadałby Twoim potrzebom za pomocą zaledwie kilku poprawek, możesz [dostosować wbudowany typ poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) Możesz na przykład dodać lub usunąć słowa kluczowe lub dodać lub usunąć dowody potwierdzające, takie jak data lub adres.
  
 **Tworzenie niestandardowego typu poufnych informacji**
  
Jeśli jednak musisz zidentyfikować i chronić zupełnie inny typ poufnych informacji, możesz [utworzyć niestandardowy typ poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika Centrum zgodności & zabezpieczeń.
  
**Tworzenie niestandardowego typu poufnych informacji w programie PowerShell centrum zabezpieczeń & Compliance Center**

Jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, można [utworzyć niestandardowy typ poufnych informacji w programie Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Zaczynając od pliku XML, można użyć każdej dostępnej opcji.
