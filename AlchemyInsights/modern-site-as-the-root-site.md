---
title: Nowoczesne witryny jako witryny głównej
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057751"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="d77ad-102">Nowoczesne witryny jako witryny głównej</span><span class="sxs-lookup"><span data-stu-id="d77ad-102">Modern site as root site</span></span>

<span data-ttu-id="d77ad-103">Klienci [Wersji docelowej](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) można włączyć teraz doświadczenie strony nowoczesnej komunikacji w miejscu głównego klasyczne ich dzierżawcy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d77ad-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="d77ad-104">Tę funkcję można aktywować za pomocą prostego polecenia cmdlet programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d77ad-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="d77ad-105">Na pomyślne wykonanie polecenia środowiska PowerShell witryny głównej ma nową stronę główną witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="d77ad-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="d77ad-106">Szczegóły dotyczące wymagań funkcji i polecenia cmdlet środowiska PowerShell są dostępne w artykule [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="d77ad-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="d77ad-107">Firma Microsoft będzie być wprowadzana stopniowo tę możliwość, off domyślnie klientom ukierunkowane zwolnienia z początku maja 2019, a roll się będzie dostępny na całym świecie do końca czerwca 2019.</span><span class="sxs-lookup"><span data-stu-id="d77ad-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="d77ad-108">Nadal odnoszą się do [Centrum wiadomości](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) dla innych nowych funkcji z nowoczesnymi.</span><span class="sxs-lookup"><span data-stu-id="d77ad-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="d77ad-109">**Ważne**: nie należy usuwać klasyczny głównej witrynie do tworzenia nowoczesnych witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="d77ad-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="d77ad-110">Nie jest to obsługiwane przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d77ad-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="d77ad-111">Usunięcie katalogu głównego witryny spowoduje, że wszystkie witryny programu SharePoint w organizacji niedostępne dla wszystkich użytkowników, dopóki Przywracanie witryny lub utworzyć nową witrynę o takim samym adresie URL.</span><span class="sxs-lookup"><span data-stu-id="d77ad-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 