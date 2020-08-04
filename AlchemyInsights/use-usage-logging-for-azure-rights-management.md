---
title: Korzystanie z rejestrowania użycia dla usługi Azure Rights Management
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555550"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="c1be8-102">Korzystanie z rejestrowania użycia dla usługi Azure Rights Management</span><span class="sxs-lookup"><span data-stu-id="c1be8-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="c1be8-103">Domyślnie rejestrowanie użycia ochrony jest włączone dla wszystkich klientów.</span><span class="sxs-lookup"><span data-stu-id="c1be8-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="c1be8-104">Dzienniki są zapisywane jako seria obiektów blob w magazynie platformy Azure dla dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="c1be8-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="c1be8-105">Po akcji ochrony może upłynąć do 15 minut dla większości dzienników do wyświetlenia.</span><span class="sxs-lookup"><span data-stu-id="c1be8-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="c1be8-106">Dzienniki użycia ochrony można użyć do:</span><span class="sxs-lookup"><span data-stu-id="c1be8-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="c1be8-107">Analizowanie analiz biznesowych</span><span class="sxs-lookup"><span data-stu-id="c1be8-107">Analyze business insights</span></span>

- <span data-ttu-id="c1be8-108">Monitoruj nadużycia</span><span class="sxs-lookup"><span data-stu-id="c1be8-108">Monitor for abuse</span></span>

- <span data-ttu-id="c1be8-109">Wykonywanie analizy kryminalistycznej</span><span class="sxs-lookup"><span data-stu-id="c1be8-109">Perform forensic analysis</span></span>

<span data-ttu-id="c1be8-110">Aby uzyskać więcej informacji, zobacz [Rejestrowanie i analizowanie użycia ochrony z usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="c1be8-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="c1be8-111">Aby uzyskać informacje na temat rejestrowania użycia klienta, zobacz [Przewodnik administracyjny: Pliki klienta usługi Azure Information Protection i rejestrowanie użycia klienta](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="c1be8-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="c1be8-112">Aby uzyskać dodatkowe informacje, zobacz:</span><span class="sxs-lookup"><span data-stu-id="c1be8-112">For additional information, see:</span></span>

- <span data-ttu-id="c1be8-113">[Usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="c1be8-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="c1be8-114">[Samouczek: Skonfiguruj ustawienia zasad usługi Azure Information Protection i utwórz nową etykietę](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c1be8-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>