---
title: Tylko do odczytu dla utrzymania komunikat podczas próby użycia programu SharePoint lub OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620733"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7417e-102">Tylko do odczytu dla utrzymania komunikat podczas próby użycia programu SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="7417e-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7417e-103">Użytkowników może pojawić się **Tylko do odczytu dla utrzymania** komunikat podczas próby użycia programu SharePoint lub OneDrive dla jednego z następujących scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="7417e-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="7417e-104">Działania planowane lub active konserwacji.</span><span class="sxs-lookup"><span data-stu-id="7417e-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="7417e-105">Sprawdź, czy je przechodząc do [Centrum wiadomości](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="7417e-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="7417e-106">Zdarzenia usługi active wysoki priorytet, który może mieć miejsce.</span><span class="sxs-lookup"><span data-stu-id="7417e-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="7417e-107">Sprawdź, czy wszystkie klasyfikatory/przypadków przechodząc do [Usługi zdrowotne](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7417e-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="7417e-108">Drobne automatyczne naprawianie odzyskiwania scenariusz, który może się dziać z powodu nieprzewidzianych zdarzeń na serwerach, które może trwać krócej niż 30 minut lub tak.</span><span class="sxs-lookup"><span data-stu-id="7417e-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="7417e-109">Istnieją nie Centrum wiadomości lub służbie zdrowia księguje te niewielkie kwoty odzyskane, ale należy się do normalnego bardzo szybko.</span><span class="sxs-lookup"><span data-stu-id="7417e-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="7417e-110">W bardzo nielicznych przypadkach Zauważyliśmy, że jeden z trzech opisanych wyżej był przyczyną i usługa została przywrócona, ale pamięci podręcznej przeglądarki użytkowników nie zostały uporządkowane.</span><span class="sxs-lookup"><span data-stu-id="7417e-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="7417e-111">Spróbuj wyczyścić pamięć podręczną przeglądarki przed nawigowania do witryny.</span><span class="sxs-lookup"><span data-stu-id="7417e-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7417e-112">W przeglądarce Microsoft Edge wybierz **Ustawienia**, a następnie wybierz **Prywatność i Bezpieczeństwo**.</span><span class="sxs-lookup"><span data-stu-id="7417e-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7417e-113">W obszarze **Przeglądanie wyczyść**wybierz opcję **Wybierz elementy do wyczyszczenia**.</span><span class="sxs-lookup"><span data-stu-id="7417e-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7417e-114">Wybierz **pliki cookie i zapisane dane witryn internetowych**, a następnie wybierz **Wyczyść**.</span><span class="sxs-lookup"><span data-stu-id="7417e-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7417e-115">Te kroki mogą się różnić, jeżeli używasz innej przeglądarki, takich jak Google Chrome lub Mozilla Firefox.</span><span class="sxs-lookup"><span data-stu-id="7417e-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7417e-116">Innym rozwiązaniem byłoby otworzyć witryny programu SharePoint lub OneDrive w nowym oknie InPrivate.</span><span class="sxs-lookup"><span data-stu-id="7417e-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>