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
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0a412-102">Konfigurowanie ochrony przed utratą danych punktu końcowego</span><span class="sxs-lookup"><span data-stu-id="0a412-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0a412-103">Ochrona przed utratą danych firmy Microsoft umożliwia objęcie ochroną i możliwością monitorowania informacji poufnych na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0a412-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0a412-104">Po dołączeniu urządzeń do zarządzania urządzeniami możesz utworzyć zasady ochrony przed utratą danych w celu wymuszenia działań ochronnych na elementach.</span><span class="sxs-lookup"><span data-stu-id="0a412-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0a412-105">Do monitorowania aktywności w przypadku elementów poufnych można używać Eksploratora aktywności.</span><span class="sxs-lookup"><span data-stu-id="0a412-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0a412-106">W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń do zarządzania urządzeniami](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="0a412-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0a412-107">Aby rozpocząć pracę z ochroną przed utratą danych punktu końcowego:</span><span class="sxs-lookup"><span data-stu-id="0a412-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0a412-108">Upewnij się, że posiadasz odpowiednie licencjonowanie subskrypcji/jednostkę SKU.</span><span class="sxs-lookup"><span data-stu-id="0a412-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0a412-109">W celu uzyskania dodatkowych informacji zobacz [Licencjonowanie subskrypcji/jednostki SKU](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="0a412-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0a412-110">Sprawdź uprawnienia wymagane do uaktywnienia zarządzania urządzeniami, uzyskiwania dostępu do strony dołączania lub włączania/wyłączania monitorowania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="0a412-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0a412-111">Aby uzyskać więcej informacji, zobacz [Uprawnienia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="0a412-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0a412-112">Dołącz urządzenia do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="0a412-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0a412-113">W przypadku braku opcji Dołączanie urządzeń (wersja zapoznawcza) w obszarze **Ustawienia** zgodności platformy M365 potwierdź, że posiadasz odpowiednią licencję i uprawnienia, o których mowa powyżej.</span><span class="sxs-lookup"><span data-stu-id="0a412-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="0a412-114">W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="0a412-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0a412-115">Utwórz zasady ochrony przed utratą danych w celu zapewnienia ochrony elementów poufnych.</span><span class="sxs-lookup"><span data-stu-id="0a412-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0a412-116">Aby uzyskać informacje, zobacz [Scenariusze dotyczące zasad ochrony przed utratą danych punktu końcowego](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0a412-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="0a412-117">W celu uzyskania dodatkowych informacji na temat ochrony przed utratą danych punktu końcowego firmy Microsoft, zobacz [Informacje o ochronie przed utratą danych punktu końcowego platformy Microsoft 365 (wersja zapoznawcza)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="0a412-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="0a412-118">**Czynności dotyczące gromadzenia ważnych danych, jeśli potrzebna jest pomoc techniczna:**</span><span class="sxs-lookup"><span data-stu-id="0a412-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="0a412-119">Pobierz narzędzie Analizator klienta MDATP (wersja zapoznawcza) z [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="0a412-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="0a412-120">Uruchom narzędzie jako administrator w oknie wiersza poleceń:</span><span class="sxs-lookup"><span data-stu-id="0a412-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="0a412-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="0a412-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="0a412-122">W przypadku wyświetlenia monitu o treści „Enter the number of minutes to collect traces:”, wprowadź liczbę minut wymaganą do uruchomienia scenariusza</span><span class="sxs-lookup"><span data-stu-id="0a412-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="0a412-123">Uruchom scenariusz</span><span class="sxs-lookup"><span data-stu-id="0a412-123">Run the scenario</span></span>

<span data-ttu-id="0a412-124">Zbierz dane wynikowe pliku ZIP, które należy przekazać agentowi obsługi technicznej.</span><span class="sxs-lookup"><span data-stu-id="0a412-124">Collect the Zip file output to be given to the Support agent.</span></span>
