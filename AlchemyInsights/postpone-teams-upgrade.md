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
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Jak odłożyć uaktualnienie aplikacji Teams opartej na firmie Microsoft

**Ważne:** możemy rozwiązać ten problem za Pomocą narzędzia diagnostycznego pomocy technicznej, ale wygląda na to, że nie korzystasz z nowego centrum administracyjnego. Aby skorzystać z nowego centrum administracyjnego, przesuń przełącznik w prawym górnym rogu z treścią **Nowe centrum** administracyjne w prawo. Za pomocą nowego centrum administracyjnego kliknij widżet Potrzebujesz **pomocy?,** wpisz "Odrocz uaktualnienie aplikacji Teams", a następnie postępuj zgodnie z monitami, aby uruchomić diagnostykę.

Jeśli otrzymano komunikat o zautomatyzowanym uaktualnieniu aplikacji Skype dla firm firmy Microsoft do aplikacji Microsoft Teams i chcesz odłożyć automatyczne uaktualnienie na później, administrator globalny może zalogować się do portalu administracyjnego aplikacji [Teams](https://admin.teams.microsoft.com/dashboard) i po wybraniu przycisku **Odśwież stan** w obszarze Uaktualnienia aplikacji Microsoft Teams wybrać przycisk Odrocz.  Aby zobaczyć nową datę automatycznego uaktualnienia dzierżawy do usługi Microsoft Teams, odśwież stronę portalu administracyjnego aplikacji Teams.

**Uwaga:** Przycisk **Odrocz** będzie dostępny tylko w przypadku, gdy otrzymano powiadomienie centrum wiadomości dotyczące automatycznego uaktualniania. 

Administratorzy globalni mogą również uruchomić usługę [Get-CsTeamsUpgradeStatus,](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) aby dowiedzieć się więcej o ich bieżącym stanie uaktualnienia.
