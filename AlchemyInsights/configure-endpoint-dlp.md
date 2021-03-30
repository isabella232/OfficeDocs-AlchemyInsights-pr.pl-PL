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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402443"
---
# <a name="configure-endpoint-dlp"></a>Konfigurowanie ochrony przed utratą danych punktu końcowego

Ochrona przed utratą danych firmy Microsoft umożliwia objęcie ochroną i możliwością monitorowania informacji poufnych na urządzeniach z systemem Windows 10. Po dołączeniu urządzeń do zarządzania urządzeniami możesz utworzyć zasady ochrony przed utratą danych w celu wymuszenia działań ochronnych na elementach. Do monitorowania aktywności w przypadku elementów poufnych można używać Eksploratora aktywności. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń do zarządzania urządzeniami](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Aby rozpocząć pracę z ochroną przed utratą danych punktu końcowego:

- Upewnij się, że posiadasz odpowiednie licencjonowanie subskrypcji/jednostkę SKU. W celu uzyskania dodatkowych informacji zobacz [Licencjonowanie subskrypcji/jednostki SKU](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Sprawdź uprawnienia wymagane do uaktywnienia zarządzania urządzeniami, uzyskiwania dostępu do strony dołączania lub włączania/wyłączania monitorowania urządzeń. Aby uzyskać więcej informacji, zobacz [Uprawnienia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Dołącz urządzenia do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń. W przypadku braku opcji Dołączanie urządzeń (wersja zapoznawcza) w obszarze **Ustawienia** zgodności platformy M365 potwierdź, że posiadasz odpowiednią licencję i uprawnienia, o których mowa powyżej. W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Utwórz zasady ochrony przed utratą danych w celu zapewnienia ochrony elementów poufnych. Aby uzyskać informacje, zobacz [Scenariusze dotyczące zasad ochrony przed utratą danych punktu końcowego](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

W celu uzyskania dodatkowych informacji na temat ochrony przed utratą danych punktu końcowego firmy Microsoft, zobacz [Informacje o ochronie przed utratą danych punktu końcowego platformy Microsoft 365 (wersja zapoznawcza)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Czynności dotyczące gromadzenia ważnych danych, jeśli potrzebna jest pomoc techniczna:**

1. Pobierz narzędzie Analizator klienta MDATP (wersja zapoznawcza) z [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Uruchom narzędzie jako administrator w oknie wiersza poleceń:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. W przypadku wyświetlenia monitu o treści „Enter the number of minutes to collect traces:”, wprowadź liczbę minut wymaganą do uruchomienia scenariusza
5. Uruchom scenariusz

Zbierz dane wynikowe pliku ZIP, które należy przekazać agentowi obsługi technicznej.
