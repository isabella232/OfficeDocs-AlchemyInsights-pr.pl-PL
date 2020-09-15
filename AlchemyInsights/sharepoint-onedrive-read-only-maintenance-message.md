---
title: Komunikat o konserwacji — tylko do odczytu podczas próby użycia programu SharePoint lub usługi OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670842"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="f1d1c-102">Komunikat o konserwacji — tylko do odczytu podczas próby użycia programu SharePoint lub usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1d1c-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="f1d1c-103">Po próbie użycia programu SharePoint lub usługi OneDrive może zostać wyświetlony komunikat **"tylko do odczytu"** w przypadku jednego z poniższych scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="f1d1c-104">Planowana lub aktywna aktywność konserwacyjna.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="f1d1c-105">Wyszukaj je, przechodząc do [centrum wiadomości](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="f1d1c-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="f1d1c-106">Wysoki priorytet aktywnego incydentu usługowego, który może wystąpić.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="f1d1c-107">Sprawdź, czy są jakieś doradcy/incydenty, przechodząc do [kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f1d1c-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="f1d1c-108">Nieznaczny scenariusz automatycznej naprawy, który może być spowodowany nieoczekiwanymi zdarzeniami na serwerach, które mogą trwać krócej niż 30 minut.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="f1d1c-109">W przypadku tych drobnych rekondycji nie ma żadnych punktów w centrum wiadomości lub kondycji usługi, ale należy szybko wrócić do normalnego.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="f1d1c-110">W bardzo niewielkich przypadkach zaobserwowano, że jedna z trzech opisanych powyżej scenariuszy była przyczyną, a usługa została przywrócona, ale pamięć podręczna przeglądarki użytkownicy nie została wyczyszczona.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="f1d1c-111">Spróbuj wyczyścić pamięć podręczną przeglądarki przed przejściem do witryny.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="f1d1c-112">W przeglądarce programu Microsoft Edge wybierz pozycję **Ustawienia**, a następnie wybierz pozycję **prywatność i zabezpieczenia**.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="f1d1c-113">W obszarze **Wyczyść przeglądanie**wybierz pozycję **Wybierz, co chcesz wyczyścić**.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="f1d1c-114">Wybierz pozycję **pliki cookie i zapisane dane witryny sieci Web**, a następnie wybierz pozycję **Wyczyść**.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="f1d1c-115">Te czynności mogą się różnić w przypadku korzystania z innych przeglądarek, takich jak Mozilla Firefox czy Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="f1d1c-116">Inną opcją może być otwarcie witryny programu SharePoint lub usługi OneDrive w nowym oknie InPrivate.</span><span class="sxs-lookup"><span data-stu-id="f1d1c-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>