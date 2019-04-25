---
title: Włącz ATP Office 365 dla programu SharePoint, OneDrive i zespołów firmy Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403043"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="66fe5-102">Włącz pakietu Office 365 zaawansowaną ochronę przed zagrożeniami dla programu SharePoint w trybie Online, OneDrive i zespołów firmy Microsoft</span><span class="sxs-lookup"><span data-stu-id="66fe5-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="66fe5-103">Przejdź do https://protection.office.com i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="66fe5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="66fe5-104">Wybierz opcję **Zarządzanie zagrożeniami** > **zasad** > **Bezpieczne załączniki**.</span><span class="sxs-lookup"><span data-stu-id="66fe5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="66fe5-105">Wybierz opcję **Włącz ATP, SharePoint, usługi i zespoły pracowników firmy Microsoft**, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="66fe5-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="66fe5-106">(Zalecane) Jako administratora globalnego lub administratora programu SharePoint w trybie Online należy uruchomić polecenie cmdlet [Set SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** ustawionym na *wartość true*.</span><span class="sxs-lookup"><span data-stu-id="66fe5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="66fe5-107">(Zalecane) [Ustaw alerty](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dla wykrytych plików.</span><span class="sxs-lookup"><span data-stu-id="66fe5-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="66fe5-108">ATP będzie nto skanowania każdy pojedynczy plik programu SharePoint w trybie Online, OneDrive lub Teams firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="66fe5-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="66fe5-109">Pliki są skanowane asynchronicznie, poprzez proces, który używa udostępniania i Gość zdarzeń aktywności, wraz z heurystyki inteligentnego i sygnały zagrożenie do identyfikacji szkodliwych plików.</span><span class="sxs-lookup"><span data-stu-id="66fe5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="66fe5-110">Zobacz [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="66fe5-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>