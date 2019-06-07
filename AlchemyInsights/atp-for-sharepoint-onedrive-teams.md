---
title: ATP dla programu SharePoint, OneDrive i zespołów firmy Microsoft
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765278"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="46084-102">ATP dla programu SharePoint, OneDrive i zespołów firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="46084-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="46084-103">Wykonaj następujące kroki, aby włączyć zaawansowane ochronę przed zagrożeniami:</span><span class="sxs-lookup"><span data-stu-id="46084-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="46084-104">Przejdź do [https://protection.office.com](https://protection.office.com) i zaloguj się za pomocą administratora globalnego lub administratora zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="46084-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="46084-105">W lewym okienku nawigacji w obszarze **zarządzania zagrożeniem**, wybierz **zasadę** \> **Bezpieczne załączniki**.</span><span class="sxs-lookup"><span data-stu-id="46084-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="46084-106">Zaznacz opcję **Włącz ATP, SharePoint, usługi i zespoły pracowników firmy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="46084-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="46084-107">[Tworzenie alertów zasad działania](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) do otrzymywać powiadomienia, gdy zostanie wykryte szkodliwe pliki.</span><span class="sxs-lookup"><span data-stu-id="46084-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="46084-108">Aby uzyskać pełne instrukcje zobacz [temat](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="46084-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="46084-109">**Uwaga**: zgodnie z projektem ATP nie skanuje każdego z plików w programie SharePoint w trybie Online, OneDrive dla firm lub Teams Microsoft.</span><span class="sxs-lookup"><span data-stu-id="46084-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="46084-110">Pliki są skanowane asynchronicznie w procesie, który używa udostępniania działania, działanie gościa, a sygnały zagrożenia w celu identyfikacji szkodliwych plików.</span><span class="sxs-lookup"><span data-stu-id="46084-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="46084-111">Aby uzyskać więcej informacji zobacz w tym [temacie](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="46084-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
