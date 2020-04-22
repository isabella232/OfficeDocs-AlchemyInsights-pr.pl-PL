---
title: Włączanie usługi Office 365 ATP dla programu SharePoint, usługi OneDrive i usługi Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703436"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="6a4bc-102">Włączanie zaawansowanej ochrony przed zagrożeniami usługi Office 365 dla usługi SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6a4bc-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="6a4bc-103">Przejdź https://protection.office.com do i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="6a4bc-104">Wybierz pozycję Bezpieczne załączniki**zasad** >  **zarządzania zagrożeniami** > .**Safe Attachments**</span><span class="sxs-lookup"><span data-stu-id="6a4bc-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="6a4bc-105">Wybierz **pozycję Włącz atp dla programu SharePoint, OneDrive i Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="6a4bc-106">(Zalecane) Jako administrator globalny lub administrator usługi SharePoint Online uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **Nieustawianie InfectedFileDownload** ustawionym na *wartość true*.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="6a4bc-107">(Zalecane) [Skonfiguruj alerty](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczące wykrytych plików.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="6a4bc-108">Narzędzie ATP będzie skanować każdy plik w usłudze SharePoint Online, OneDrive lub usłudze Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="6a4bc-109">Pliki są skanowane asynchronicznie, za pośrednictwem procesu, który używa udostępniania i zdarzeń aktywności gościa, wraz z inteligentną heurystyką i sygnałami zagrożeń do identyfikacji złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="6a4bc-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="6a4bc-110">Zobacz [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="6a4bc-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>