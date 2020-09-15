---
title: Funkcja DLP może wymagać typu niestandardowego
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712194"
---
# <a name="dlp-might-need-a-custom-type"></a>Funkcja DLP może wymagać typu niestandardowego

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Funkcja DLP może wymagać niestandardowego typu informacji**

Dzięki zasadom ochrony przed utratą danych (DLP) można identyfikować i chronić poufne dane w organizacji. W przypadku kilku scenariuszy może być konieczne **utworzenie własnych typów informacji poufnych,** aby chronić dane organizacji.

Na przykład organizacja może potrzebować identyfikacji i ochrony identyfikatorów pracowników lub innych danych w pewnym formacie specyficznym dla organizacji. Jeśli tak, zobacz poniższe artykuły, aby uzyskać więcej informacji.
  
 **Dostosowywanie wbudowanego typu informacji poufnych**
  
Jeśli wbudowany typ informacji poufnych spełnia Twoje potrzeby, wystarczy kilka ulepszeń, aby [dostosować wbudowany typ informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Możesz na przykład dodawać lub usuwać słowa kluczowe albo dodawać lub usuwać dowody dodatkowe, takie jak data lub adres.
  
 **Tworzenie niestandardowego typu informacji poufnych**
  
Jeśli jednak konieczne jest całkowite zidentyfikowanie i chronienie różnych typów poufnych informacji, można [utworzyć niestandardowe typy informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika centrum zabezpieczeń & zgodności.
  
**Tworzenie niestandardowego typu informacji poufnych w centrum zabezpieczeń & zgodności programu PowerShell**

Na koniec, jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, możesz [utworzyć niestandardowy typ informacji poufnych w centrum zabezpieczeń & zgodności programu PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Rozpoczynając od pliku XML, możesz korzystać z każdej dostępnej opcji.
