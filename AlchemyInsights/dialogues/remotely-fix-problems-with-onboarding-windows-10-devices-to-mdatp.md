---
title: Zdalne rozwiązywanie problemów z dołączaniem urządzeń z systemem Windows 10 do usługi Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694850"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="ce395-102">Zdalne rozwiązywanie problemów z dołączaniem urządzeń z systemem Windows 10 do usługi Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="ce395-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="ce395-103">Jeśli możesz uzyskać dostęp do komputera zdalnego, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ce395-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="ce395-104">Pobierz narzędzie [diagnostyczne Analizator łączności z klientem.](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="ce395-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="ce395-105">Wyodrębnianie i uruchamianie pliku MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="ce395-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="ce395-106">Znajdź dziennik diagnostyczny w folderze MDATPClientAnalyzerResult, który jest tym samym folderem, w którym pobrano narzędzie Analizator.</span><span class="sxs-lookup"><span data-stu-id="ce395-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="ce395-107">Aby znaleźć problemy z łącznością lub ustawieniami internetowego serwera proxy, przejrzyj plik MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="ce395-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="ce395-108">Aby dowiedzieć się więcej, zobacz [Problemy z komputerami dołączania.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="ce395-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
