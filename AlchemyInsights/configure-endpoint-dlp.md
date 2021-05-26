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
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3c35f-102">Konfigurowanie ochrony przed utratą danych punktu końcowego</span><span class="sxs-lookup"><span data-stu-id="3c35f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3c35f-103">Ochrona przed utratą danych firmy Microsoft umożliwia objęcie ochroną i możliwością monitorowania informacji poufnych na urządzeniach z systemem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3c35f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3c35f-104">Po dołączeniu urządzeń do zarządzania urządzeniami możesz utworzyć zasady ochrony przed utratą danych w celu wymuszenia działań ochronnych na elementach.</span><span class="sxs-lookup"><span data-stu-id="3c35f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3c35f-105">Do monitorowania aktywności w przypadku elementów poufnych można używać Eksploratora aktywności.</span><span class="sxs-lookup"><span data-stu-id="3c35f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3c35f-106">W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń do zarządzania urządzeniami](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="3c35f-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3c35f-107">Aby rozpocząć pracę z ochroną przed utratą danych punktu końcowego:</span><span class="sxs-lookup"><span data-stu-id="3c35f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3c35f-108">Upewnij się, że posiadasz odpowiednie licencjonowanie subskrypcji/jednostkę SKU.</span><span class="sxs-lookup"><span data-stu-id="3c35f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3c35f-109">W celu uzyskania dodatkowych informacji zobacz [Licencjonowanie subskrypcji/jednostki SKU](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="3c35f-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3c35f-110">Sprawdź uprawnienia wymagane do uaktywnienia zarządzania urządzeniami, uzyskiwania dostępu do strony dołączania lub włączania/wyłączania monitorowania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="3c35f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="3c35f-111">Aby uzyskać więcej informacji, zobacz [Uprawnienia](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="3c35f-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3c35f-112">Dołącz urządzenia do zarządzania urządzeniami, wykonując procedurę dołączania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="3c35f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3c35f-113">W celu uzyskania dodatkowych informacji zobacz [Dołączanie urządzeń](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="3c35f-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3c35f-114">Utwórz zasady ochrony przed utratą danych w celu zapewnienia ochrony elementów poufnych.</span><span class="sxs-lookup"><span data-stu-id="3c35f-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3c35f-115">Aby uzyskać informacje, zobacz [Scenariusze dotyczące zasad ochrony przed utratą danych punktu końcowego](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="3c35f-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="3c35f-116">W celu uzyskania dodatkowych informacji na temat ochrony przed utratą danych punktu końcowego firmy Microsoft, zobacz [Informacje o ochronie przed utratą danych punktu końcowego platformy Microsoft 365 (wersja zapoznawcza)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="3c35f-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="3c35f-117">**Czynności dotyczące gromadzenia ważnych danych, jeśli potrzebna jest pomoc techniczna:**</span><span class="sxs-lookup"><span data-stu-id="3c35f-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="3c35f-118">Pobierz [MDATP Podgląd analizatora klientów.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="3c35f-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="3c35f-119">Uruchom narzędzie jako administrator w oknie wiersza poleceń:</span><span class="sxs-lookup"><span data-stu-id="3c35f-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="3c35f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="3c35f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="3c35f-121">Gdy zostanie wyświetlony monit Wprowadź liczbę minut na zebranie **śledzenia:**, wprowadź liczbę minut wymaganą do uruchomienia scenariusza.</span><span class="sxs-lookup"><span data-stu-id="3c35f-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="3c35f-122">Uruchom scenariusz.</span><span class="sxs-lookup"><span data-stu-id="3c35f-122">Run the scenario.</span></span>

<span data-ttu-id="3c35f-123">Zbierz dane wyjściowe pliku zip, aby przekazać je agentowi pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="3c35f-123">Collect the Zip file output to give to the Support agent.</span></span>
