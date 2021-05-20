---
title: Włączanie Office 365 ATP dla SharePoint, OneDrive i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543938"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="af315-102">Włączanie usługi Microsoft Defender Office 365 dla SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="af315-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="af315-103">Przejdź do https://protection.office.com i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="af315-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="af315-104">Wybierz **pozycję Zasady zarządzania**  >    >  **zagrożeniami Sejf załączników.**</span><span class="sxs-lookup"><span data-stu-id="af315-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="af315-105">Wybierz **pozycję Włącz defender dla Office 365 dla SharePoint, OneDrive i Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="af315-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="af315-106">(Zalecane) Jako administrator globalny lub administrator usługi SharePoint Online uruchom polecenie cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość true.*</span><span class="sxs-lookup"><span data-stu-id="af315-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="af315-107">(Zalecane) [Konfigurowanie alertów dotyczących](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) wykrytych plików.</span><span class="sxs-lookup"><span data-stu-id="af315-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="af315-108">Program Microsoft Defender dla Office 365 nie skanuje wszystkich plików w aplikacjach SharePoint Online, OneDrive i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="af315-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="af315-109">Pliki są skanowane asynchronicznie w ramach procesu, który używa zdarzeń udostępniania i aktywności gościa, a także inteligentnych heuristics i sygnałów zagrożeń do identyfikowania złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="af315-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="af315-110">Zobacz [Program Microsoft Defender, Office 365, aby SharePoint, OneDrive i Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="af315-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>