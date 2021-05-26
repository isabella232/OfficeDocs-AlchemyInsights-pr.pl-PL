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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657939"
---
# <a name="configure-endpoint-dlp"></a>Konfigurowanie ochrony przed utratą danych punktu końcowego

Ochrona przed utratą danych firmy Microsoft umożliwia objęcie ochroną i możliwością monitorowania informacji poufnych na urządzeniach z systemem Windows 10. Po dołączeniu urządzeń do zarządzania urządzeniami możesz utworzyć zasady ochrony przed utratą danych w celu wymuszenia działań ochronnych na elementach. Do monitorowania aktywności w przypadku elementów poufnych można używać Eksploratora aktywności. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń do zarządzania urządzeniami](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Aby rozpocząć pracę z ochroną przed utratą danych punktu końcowego:

- Upewnij się, że posiadasz odpowiednie licencjonowanie subskrypcji/jednostkę SKU. W celu uzyskania dodatkowych informacji zobacz [Licencjonowanie subskrypcji/jednostki SKU](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Sprawdź uprawnienia wymagane do uaktywnienia zarządzania urządzeniami, uzyskiwania dostępu do strony dołączania lub włączania/wyłączania monitorowania urządzeń. Aby uzyskać więcej informacji, zobacz [Uprawnienia](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Dołącz urządzenia do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Utwórz zasady ochrony przed utratą danych w celu zapewnienia ochrony elementów poufnych. Aby uzyskać informacje, zobacz [Scenariusze dotyczące zasad ochrony przed utratą danych punktu końcowego](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

W celu uzyskania dodatkowych informacji na temat ochrony przed utratą danych punktu końcowego firmy Microsoft, zobacz [Informacje o ochronie przed utratą danych punktu końcowego platformy Microsoft 365 (wersja zapoznawcza)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Czynności dotyczące gromadzenia ważnych danych, jeśli potrzebna jest pomoc techniczna:**

1. Pobierz [MDATP Podgląd analizatora klientów.](https://aka.ms/betamdatpanalyzer)
1. Uruchom narzędzie jako administrator w oknie wiersza poleceń:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Gdy zostanie wyświetlony monit Wprowadź liczbę minut na zebranie **śledzenia:**, wprowadź liczbę minut wymaganą do uruchomienia scenariusza.
1. Uruchom scenariusz.

Zbierz dane wyjściowe pliku zip, aby przekazać je agentowi pomocy technicznej.
