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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709917"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2fd06-102">365 Włączanie zaawansowanej ochrony przed zagrożeniami dla usługi SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2fd06-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="2fd06-103">Przejdź do https://protection.office.com i zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="2fd06-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="2fd06-104">Wybieranie **Threat management**  >  **Policy**  >  **bezpiecznych załączników**zasad zarządzania zagrożeniami.</span><span class="sxs-lookup"><span data-stu-id="2fd06-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="2fd06-105">Wybierz pozycję **Włącz ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams**, a następnie kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="2fd06-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="2fd06-106">Zalecon Jako Administrator globalny lub administrator usługi SharePoint Online Uruchom polecenie cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parametrem **DisallowInfectedFileDownload** o wartości *true*.</span><span class="sxs-lookup"><span data-stu-id="2fd06-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="2fd06-107">Zalecon [Konfigurowanie alertów](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) dotyczących wykrytych plików.</span><span class="sxs-lookup"><span data-stu-id="2fd06-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="2fd06-108">ATP usunie skanowanie każdego pojedynczego pliku w usłudze SharePoint Online, OneDrive lub Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2fd06-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="2fd06-109">Pliki są skanowane asynchronicznie za pomocą procesu, w którym są używane zdarzenia dotyczące udostępniania i aktywności gościa, a także inteligentne heurystyka i sygnały zagrożeń w celu zidentyfikowania złośliwych plików.</span><span class="sxs-lookup"><span data-stu-id="2fd06-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="2fd06-110">Zobacz [ATP dla programu SharePoint, usługi OneDrive i aplikacji Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2fd06-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>