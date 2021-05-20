---
title: Usługa Microsoft Defender dla Office 365 dla SharePoint, OneDrive i Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543587"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="46c9e-102">Usługa Microsoft Defender dla Office 365 dla SharePoint, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="46c9e-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="46c9e-103">Wykonaj poniższe czynności, aby włączyć program Microsoft Defender dla Office 365:</span><span class="sxs-lookup"><span data-stu-id="46c9e-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="46c9e-104">Przejdź do konta administratora globalnego lub administratora zabezpieczeń i [https://protection.office.com](https://protection.office.com) zaloguj się do tego konta.</span><span class="sxs-lookup"><span data-stu-id="46c9e-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="46c9e-105">W lewym okienku nawigacji w obszarze **Zarządzanie zagrożeniami** wybierz **pozycję Zasady** \> **Sejf załączników**.</span><span class="sxs-lookup"><span data-stu-id="46c9e-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="46c9e-106">Wybierz **pozycję Włącz defender dla Office 365, SharePoint, OneDrive i Microsoft Teams.**</span><span class="sxs-lookup"><span data-stu-id="46c9e-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="46c9e-107">[Utwórz zasady alertów aktywności, aby](/microsoft-365/compliance/create-activity-alerts) otrzymywać powiadomienia po wykryciu złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="46c9e-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="46c9e-108">Aby uzyskać pełne instrukcje, zobacz Włączanie [załączników Sejf załączników](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)wiadomości SharePoint, OneDrive i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="46c9e-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="46c9e-109">**Uwaga:** Program Microsoft Defender for Office 365 domyślnie nie skanuje wszystkich plików w aplikacjach SharePoint Online, OneDrive dla Firm i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="46c9e-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="46c9e-110">Pliki są skanowane asynchronicznie przez proces, który do identyfikowania złośliwych plików używa aktywności udostępniania, aktywności gościa i sygnałów zagrożeń.</span><span class="sxs-lookup"><span data-stu-id="46c9e-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="46c9e-111">Aby uzyskać więcej informacji, [zobacz Sejf załączniki do SharePoint, OneDrive i Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="46c9e-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
