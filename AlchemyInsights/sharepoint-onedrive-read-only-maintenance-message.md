---
title: Tylko do odczytu dla konserwacji komunikat podczas próby użycia programu SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051291"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="a77cd-102">Tylko do odczytu dla konserwacji komunikat podczas próby użycia programu SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="a77cd-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="a77cd-103">Użytkownicy mogą odbierać **tylko do odczytu dla komunikat konserwacji** podczas próby użycia programu SharePoint lub OneDrive dla jednego z następujących scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="a77cd-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="a77cd-104">Planowane lub aktywne czynności konserwacyjne.</span><span class="sxs-lookup"><span data-stu-id="a77cd-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="a77cd-105">Sprawdź je, przechodząc do [centrum wiadomości](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="a77cd-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="a77cd-106">Zdarzenia o wysokim priorytecie, aktywne usługi, które mogą mieć miejsce.</span><span class="sxs-lookup"><span data-stu-id="a77cd-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="a77cd-107">Sprawdź, czy nie ma żadnych porad/incydentów, przechodząc do [usługi kondycji](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a77cd-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="a77cd-108">Niewielki scenariusz odzyskiwania Auto-Healing, który może się wydarzy z powodu nieoczekiwanych zdarzeń na serwerach, które mogą trwać krócej niż 30 min lub więcej.</span><span class="sxs-lookup"><span data-stu-id="a77cd-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="a77cd-109">Nie ma żadnych wiadomości Center lub usługi zdrowia stanowisk dla tych drobnych odzyskuje, ale należy wrócić do normalnego bardzo szybko.</span><span class="sxs-lookup"><span data-stu-id="a77cd-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="a77cd-110">W bardzo niewielu przypadkach zaobserwowaliśmy, że jeden z trzech scenariuszy wymienionych powyżej był przyczyną, a usługa została przywrócona, ale pamięć podręczna przeglądarki użytkowników nie została wyczyszczona.</span><span class="sxs-lookup"><span data-stu-id="a77cd-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="a77cd-111">Spróbuj wyczyścić pamięć podręczną przeglądarki przed nawigacją do witryny.</span><span class="sxs-lookup"><span data-stu-id="a77cd-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="a77cd-112">W przeglądarce Microsoft Edge wybierz pozycję **Ustawienia**, a następnie wybierz pozycję **prywatność i zabezpieczenia**.</span><span class="sxs-lookup"><span data-stu-id="a77cd-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="a77cd-113">W obszarze **Wyczyść przeglądanie**wybierz pozycję **Wybierz, co chcesz wyczyścić**.</span><span class="sxs-lookup"><span data-stu-id="a77cd-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="a77cd-114">Wybierz **pliki cookie i zapisane dane witryny**, a następnie wybierz pozycję **Wyczyść**.</span><span class="sxs-lookup"><span data-stu-id="a77cd-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="a77cd-115">Te kroki mogą się różnić w przypadku korzystania z innych przeglądarek, takich jak Mozilla Firefox lub Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="a77cd-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="a77cd-116">Inną opcją byłoby otworzyć witrynę programu SharePoint lub OneDrive w nowym oknie InPrivate.</span><span class="sxs-lookup"><span data-stu-id="a77cd-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>