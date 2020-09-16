---
title: Uaktualnienie dotyczące odroczonego zespołu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741781"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="9c45d-102">Jak odłożyć uaktualnienie zespołów opartych na firmie Microsoft</span><span class="sxs-lookup"><span data-stu-id="9c45d-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="9c45d-103">**Ważne**: możemy pomóc rozwiązać ten problem za pomocą diagnostycznej pomocy technicznej, ale wygląda na to, że nie korzystasz z nowego centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="9c45d-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="9c45d-104">Aby użyć nowego centrum administracyjnego, przesuń przełącznik w prawo po prawej stronie od **nowego centrum administracyjnego** .</span><span class="sxs-lookup"><span data-stu-id="9c45d-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="9c45d-105">Korzystając z nowego centrum administracyjnego, kliknij widżet **potrzebujesz pomocy?** , wpisz "Odłóż uaktualnienie zespołów", a następnie postępuj zgodnie z instrukcjami, aby uruchomić diagnostykę.</span><span class="sxs-lookup"><span data-stu-id="9c45d-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="9c45d-106">Jeśli otrzymano komunikat o zautomatyzowanej aktualizacji prowadzonej przez firmę Microsoft z programu Skype dla firm do aplikacji Microsoft Teams i chcesz odłożyć automatyczne uaktualnienie do późniejszej daty, Administrator globalny może zalogować się do [portalu administrator zespołów](https://admin.teams.microsoft.com/dashboard) i po wybraniu przycisku **Odśwież stan** w obszarze uaktualnienie aplikacji Microsoft Teams wybierz przycisk **Odłóż** .</span><span class="sxs-lookup"><span data-stu-id="9c45d-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="9c45d-107">Aby wyświetlić nową datę automatycznego uaktualnienia dzierżawy do aplikacji Microsoft Teams, Odśwież stronę portalu administrator zespołów.</span><span class="sxs-lookup"><span data-stu-id="9c45d-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="9c45d-108">**Uwaga:** Przycisk **Odłóż** będzie dostępny tylko wtedy, gdy otrzymano powiadomienie dotyczące automatycznego uaktualnienia w centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="9c45d-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="9c45d-109">Administratorzy globalni mogą również uruchomić polecenie [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , aby dowiedzieć się więcej o aktualnym stanie uaktualnienia.</span><span class="sxs-lookup"><span data-stu-id="9c45d-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
