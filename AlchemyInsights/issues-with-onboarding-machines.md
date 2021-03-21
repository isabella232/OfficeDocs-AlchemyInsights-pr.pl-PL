---
title: Problemy z dołączaniem komputerów do usługi Zaawansowana ochrona przed zagrożeniami w usłudze Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901577"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="e937f-102">Problemy z dołączaniem komputerów do usługi Zaawansowana ochrona przed zagrożeniami w usłudze Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="e937f-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="e937f-103">Mogą występować problemy z dołączaniem komputerów do usługi Zaawansowana ochrona przed zagrożeniami w usłudze Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="e937f-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="e937f-104">Jeśli możesz uzyskać dostęp do komputera użytkownika końcowego, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="e937f-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="e937f-105">Pobierz najnowszą wersję zapoznawczą narzędzia diagnostycznego [Analizator klienta MDE](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="e937f-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="e937f-106">Kliknij plik **MDEClientAnalyzer.cmd** prawym przyciskiem myszy i wybierz opcję „Uruchom jako administrator”.</span><span class="sxs-lookup"><span data-stu-id="e937f-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="e937f-107">Postępuj zgodnie ze wskazówkami wyświetlanymi w pliku **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="e937f-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="e937f-108">W celu uzyskania bardziej szczegółowych dzienników, przejrzyj utworzony podfolder o nazwie **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="e937f-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="e937f-109">Jeśli potrzebne są dodatkowe wskazówki, skontaktuj się z [pomocą techniczną usługi Zaawansowana ochrona przed zagrożeniami w usłudze Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) i przekaż plik wynikowy MDEClientAnalyzerResult.zip na potrzeby analizy.</span><span class="sxs-lookup"><span data-stu-id="e937f-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
