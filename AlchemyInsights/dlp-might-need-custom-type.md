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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446701"
---
# <a name="dlp-might-need-a-custom-type"></a>W przypadku zasad DLP może być potrzebny typ niestandardowy

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP może wymagać niestandardowego typu informacji**

Przy użyciu zasad ochrony przed utratą danych (DLP, data loss prevention) możesz identyfikować i chronić poufne dane w swojej organizacji. W niektórych scenariuszach może być konieczne utworzenie własnego niestandardowego typu informacji poufnych w celu ochrony danych organizacji. Aby uzyskać więcej informacji, zobacz [Informacje o typach informacji poufnych i](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) definicjach [encji typu informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Aby uzyskać więcej informacji na temat tworzenia niestandardowych typów i zasad dotyczących informacji poufnych, zobacz: 

**Dostosowywanie wbudowanego typu informacji poufnych**

Jeśli wbudowany typ informacji poufnych spełni Twoje potrzeby za pomocą zaledwie kilku ulepszeń, zobacz Dostosowywanie wbudowanego typu informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Na przykład można dodawać lub usuwać słowa kluczowe albo dodawać lub usuwać informacje dodatkowe, takie jak data lub adres.

**Tworzenie niestandardowego typu informacji poufnych**

Jeśli jednak musisz całkowicie zidentyfikować i chronić inny typ informacji poufnych, możesz utworzyć niestandardowy typ informacji poufnych w Centrum zgodności platformy Microsoft 365. Aby uzyskać więcej informacji, zobacz [Wprowadzenie do niestandardowych typów informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Tworzenie niestandardowego typu informacji poufnych w programie PowerShell & w Centrum zgodności**

Jeśli interfejs użytkownika nie zawiera wszystkich potrzebnych opcji, można utworzyć niestandardowy typ informacji poufnych w programie PowerShell centrum zabezpieczeń & zgodności. Zaczynając od pliku XML, możesz użyć wszystkich dostępnych opcji. Aby uzyskać więcej informacji, zobacz Tworzenie niestandardowego typu informacji [poufnych przy użyciu programu PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Aby najpierw przetestować zasady w trybie testowania, zobacz [Implementowanie zasad](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) w trybie testowania oraz [Tworzenie, testowanie i dostosowywanie zasad DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 