---
title: Odkładanie Teams uaktualnianie
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
ms.openlocfilehash: 893a01ae74f8aec9bb0079430188e3cd6881b3009818830ea5572cfa41cdf71f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923987"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Jak odłożyć aktualizację kierowaną przez Teams Microsoft

**Ważne:** możemy rozwiązać ten problem za Pomocą narzędzia diagnostycznego pomocy technicznej, ale wygląda na to, że nie korzystasz z nowego centrum administracyjnego. Aby skorzystać z nowego centrum administracyjnego, przesuń przełącznik w prawym górnym rogu z treścią **Nowe centrum** administracyjne w prawo. Za pomocą nowego centrum administracyjnego kliknij widżet Potrzebujesz **pomocy?,** wpisz "Odrocz Teams uaktualnianie", a następnie postępuj zgodnie z monitami, aby uruchomić narzędzie diagnostyczne.

Jeśli otrzymano informacje o automatycznym uaktualnieniu prowadzonym przez firmę Microsoft z programu Skype dla firm do programu Microsoft Teams i chcesz odłożyć automatyczne uaktualnienie na później, administrator  globalny może zalogować się do  portalu administratora programu [Teams](https://admin.teams.microsoft.com/dashboard) i po wybraniu przycisku Odśwież stan w obszarze Uaktualnianie do usługi Microsoft Teams wybrać przycisk Odrocz. Aby zobaczyć nową datę automatycznego uaktualnienia dzierżawy do nowej Microsoft Teams, odśwież stronę Teams administracyjnej.

**Uwaga:** Przycisk **Odrocz** będzie dostępny tylko w przypadku, gdy otrzymano powiadomienie centrum wiadomości dotyczące automatycznego uaktualniania. 

Administratorzy globalni mogą również uruchomić usługę [Get-CsTeamsUpgradeStatus,](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) aby dowiedzieć się więcej o ich bieżącym stanie uaktualnienia.
