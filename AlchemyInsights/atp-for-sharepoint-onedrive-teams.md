---
title: ATP dla programu SharePoint, OneDrive i Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712468"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="9af9a-102">ATP dla programu SharePoint, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9af9a-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="9af9a-103">Wykonaj następujące kroki, aby włączyć zaawansowaną ochronę przed zagrożeniami:</span><span class="sxs-lookup"><span data-stu-id="9af9a-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="9af9a-104">Przejdź [https://protection.office.com](https://protection.office.com) do konta administratora globalnego lub administratora zabezpieczeń i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="9af9a-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="9af9a-105">W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami**wybierz pozycję **Załączniki bezpieczne dla** **zasad** \> .</span><span class="sxs-lookup"><span data-stu-id="9af9a-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="9af9a-106">Wybierz **pozycję Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="9af9a-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="9af9a-107">[Utwórz zasady alertów aktywności,](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) aby otrzymywać powiadomienia, gdy wykryjemy złośliwe pliki.</span><span class="sxs-lookup"><span data-stu-id="9af9a-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="9af9a-108">Aby uzyskać pełne instrukcje, zobacz ten [temat](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9af9a-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="9af9a-109">**Uwaga:** Zgodnie z projektem narzędzie ATP nie skanuje każdego pliku w usłudze SharePoint Online, usłudze OneDrive dla Firm ani w usłudze Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9af9a-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="9af9a-110">Pliki są skanowane asynchronicznie przez proces, który używa aktywności udostępniania, aktywności gościa i sygnałów zagrożeń do identyfikowania złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="9af9a-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="9af9a-111">Aby uzyskać więcej informacji, zobacz ten [temat](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9af9a-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
