---
title: Konfigurowanie ochrony przed utratą danych punktu końcowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892809"
---
# <a name="configure-endpoint-dlp"></a>Konfigurowanie ochrony przed utratą danych punktu końcowego

Ochrona przed utratą danych firmy Microsoft umożliwia objęcie ochroną i możliwością monitorowania informacji poufnych na urządzeniach z systemem Windows 10. Po dołączeniu urządzeń do zarządzania urządzeniami możesz utworzyć zasady ochrony przed utratą danych w celu wymuszenia działań ochronnych na elementach. Do monitorowania aktywności w przypadku elementów poufnych można używać Eksploratora aktywności. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń do zarządzania urządzeniami](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Aby rozpocząć pracę z ochroną przed utratą danych punktu końcowego:

- Upewnij się, że posiadasz odpowiednie licencjonowanie subskrypcji/jednostkę SKU. W celu uzyskania dodatkowych informacji zobacz [Licencjonowanie subskrypcji/jednostki SKU](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Sprawdź uprawnienia wymagane do uaktywnienia zarządzania urządzeniami, uzyskiwania dostępu do strony dołączania lub włączania/wyłączania monitorowania urządzeń. Aby uzyskać więcej informacji, zobacz [Uprawnienia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Dołącz urządzenia do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Utwórz zasady ochrony przed utratą danych w celu zapewnienia ochrony elementów poufnych. Aby uzyskać informacje, zobacz [Scenariusze dotyczące zasad ochrony przed utratą danych punktu końcowego](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

W celu uzyskania dodatkowych informacji na temat ochrony przed utratą danych punktu końcowego firmy Microsoft, zobacz [Informacje o ochronie przed utratą danych punktu końcowego platformy Microsoft 365 (wersja zapoznawcza)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Czynności dotyczące gromadzenia ważnych danych, jeśli potrzebna jest pomoc techniczna:**

1. Pobierz [podgląd analizatora klienta MDATP.](https://aka.ms/betamdatpanalyzer)
1. Uruchom narzędzie jako administrator w oknie wiersza poleceń:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Gdy zostanie wyświetlony monit Wprowadź liczbę minut na zebranie **śledzenia:**, wprowadź liczbę minut wymaganą do uruchomienia scenariusza.
1. Uruchom scenariusz.

Zbierz dane wyjściowe pliku zip, aby przekazać je agentowi pomocy technicznej.
