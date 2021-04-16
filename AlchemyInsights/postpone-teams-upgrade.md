---
title: Odkładanie uaktualnienia aplikacji Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801241"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="93fcf-102">Jak odłożyć uaktualnienie aplikacji Teams opartej na firmie Microsoft</span><span class="sxs-lookup"><span data-stu-id="93fcf-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="93fcf-103">**Ważne:** możemy rozwiązać ten problem za Pomocą narzędzia diagnostycznego pomocy technicznej, ale wygląda na to, że nie korzystasz z nowego centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="93fcf-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="93fcf-104">Aby skorzystać z nowego centrum administracyjnego, przesuń przełącznik w prawym górnym rogu z treścią **Nowe centrum** administracyjne w prawo.</span><span class="sxs-lookup"><span data-stu-id="93fcf-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="93fcf-105">Za pomocą nowego centrum administracyjnego kliknij widżet Potrzebujesz **pomocy?,** wpisz "Odrocz uaktualnienie aplikacji Teams", a następnie postępuj zgodnie z monitami, aby uruchomić diagnostykę.</span><span class="sxs-lookup"><span data-stu-id="93fcf-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="93fcf-106">Jeśli otrzymano komunikat o zautomatyzowanym uaktualnieniu aplikacji Skype dla firm firmy Microsoft do aplikacji Microsoft Teams i chcesz odłożyć automatyczne uaktualnienie na później, administrator globalny może zalogować się do portalu administracyjnego aplikacji [Teams](https://admin.teams.microsoft.com/dashboard) i po wybraniu przycisku **Odśwież stan** w obszarze Uaktualnienia aplikacji Microsoft Teams wybrać przycisk Odrocz. </span><span class="sxs-lookup"><span data-stu-id="93fcf-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="93fcf-107">Aby zobaczyć nową datę automatycznego uaktualnienia dzierżawy do usługi Microsoft Teams, odśwież stronę portalu administracyjnego aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="93fcf-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="93fcf-108">**Uwaga:** Przycisk **Odrocz** będzie dostępny tylko w przypadku, gdy otrzymano powiadomienie centrum wiadomości dotyczące automatycznego uaktualniania.</span><span class="sxs-lookup"><span data-stu-id="93fcf-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="93fcf-109">Administratorzy globalni mogą również uruchomić usługę [Get-CsTeamsUpgradeStatus,](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) aby dowiedzieć się więcej o ich bieżącym stanie uaktualnienia.</span><span class="sxs-lookup"><span data-stu-id="93fcf-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
