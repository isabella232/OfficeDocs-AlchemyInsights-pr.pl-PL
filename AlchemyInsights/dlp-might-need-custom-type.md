---
title: W przypadku zasad DLP może być potrzebny typ niestandardowy
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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030804"
---
# <a name="dlp-might-need-a-custom-type"></a>W przypadku zasad DLP może być potrzebny typ niestandardowy

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP może wymagać niestandardowego typu informacji**

Przy użyciu zasad ochrony przed utratą danych (DLP, data loss prevention) możesz identyfikować i chronić poufne dane w swojej organizacji. W niektórych scenariuszach może być  konieczne utworzenie własnego niestandardowego typu informacji poufnych w celu ochrony danych organizacji.

Na przykład organizacja może wymagać zidentyfikowania i ochrony identyfikatorów pracowników lub innych danych w innym formacie, specyficznym dla Twojej organizacji. Jeśli tak, zapoznaj się z następującymi artykułami, aby uzyskać więcej informacji.
  
 **Dostosowywanie wbudowanego typu informacji poufnych**
  
Jeśli wbudowany typ informacji poufnych spełni Twoje potrzeby za pomocą zaledwie kilku ulepszeń, możesz dostosować wbudowany typ informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Na przykład można dodawać lub usuwać słowa kluczowe albo dodawać lub usuwać informacje dodatkowe, takie jak data lub adres.
  
 **Tworzenie niestandardowego typu informacji poufnych**
  
Jeśli jednak musisz całkowicie zidentyfikować i chronić inny typ [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) informacji poufnych, możesz utworzyć niestandardowy typ informacji poufnych w interfejsie użytkownika centrum zabezpieczeń & zgodności.
  
**Tworzenie niestandardowego typu informacji poufnych w centrum & w programie PowerShell**

Jeśli interfejs użytkownika nie zawiera wszystkich potrzebnych opcji, możesz utworzyć niestandardowy typ informacji poufnych w programie PowerShell centrum zabezpieczeń & [zgodności.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Zaczynając od pliku XML, możesz użyć wszystkich dostępnych opcji.
