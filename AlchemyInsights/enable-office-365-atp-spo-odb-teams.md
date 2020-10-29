---
title: Włącz usługę Office 365 ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801063"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ad6e2-102">Włączanie usługi Microsoft Defender dla pakietu Office 365 dla usług SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ad6e2-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ad6e2-103">Przejdź do https://protection.office.com i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="ad6e2-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ad6e2-104">Wybieranie **Threat management**  >  **Policy**  >  **bezpiecznych załączników** zasad zarządzania zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="ad6e2-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="ad6e2-105">Wybierz pozycję **Włącz ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams** , a następnie kliknij przycisk **Zapisz** .</span><span class="sxs-lookup"><span data-stu-id="ad6e2-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="ad6e2-106">Zalecon Jako Administrator globalny lub administrator usługi SharePoint Online Uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** o wartości *true* .</span><span class="sxs-lookup"><span data-stu-id="ad6e2-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="ad6e2-107">Zalecon [Konfigurowanie alertów](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczących wykrytych plików.</span><span class="sxs-lookup"><span data-stu-id="ad6e2-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ad6e2-108">ATP usunie skanowanie każdego pojedynczego pliku w usłudze SharePoint Online, OneDrive lub Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ad6e2-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ad6e2-109">Pliki są skanowane asynchronicznie za pomocą procesu, w którym są używane zdarzenia dotyczące udostępniania i aktywności gościa, a także inteligentne heurystyka i sygnały zagrożeń w celu zidentyfikowania złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="ad6e2-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ad6e2-110">Zobacz [ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ad6e2-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>