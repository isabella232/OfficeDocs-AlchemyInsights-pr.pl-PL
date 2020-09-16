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
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Jak odłożyć uaktualnienie zespołów opartych na firmie Microsoft

**Ważne**: możemy pomóc rozwiązać ten problem za pomocą diagnostycznej pomocy technicznej, ale wygląda na to, że nie korzystasz z nowego centrum administracyjnego. Aby użyć nowego centrum administracyjnego, przesuń przełącznik w prawo po prawej stronie od **nowego centrum administracyjnego** . Korzystając z nowego centrum administracyjnego, kliknij widżet **potrzebujesz pomocy?** , wpisz "Odłóż uaktualnienie zespołów", a następnie postępuj zgodnie z instrukcjami, aby uruchomić diagnostykę.

Jeśli otrzymano komunikat o zautomatyzowanej aktualizacji prowadzonej przez firmę Microsoft z programu Skype dla firm do aplikacji Microsoft Teams i chcesz odłożyć automatyczne uaktualnienie do późniejszej daty, Administrator globalny może zalogować się do [portalu administrator zespołów](https://admin.teams.microsoft.com/dashboard) i po wybraniu przycisku **Odśwież stan** w obszarze uaktualnienie aplikacji Microsoft Teams wybierz przycisk **Odłóż** . Aby wyświetlić nową datę automatycznego uaktualnienia dzierżawy do aplikacji Microsoft Teams, Odśwież stronę portalu administrator zespołów.

**Uwaga:** Przycisk **Odłóż** będzie dostępny tylko wtedy, gdy otrzymano powiadomienie dotyczące automatycznego uaktualnienia w centrum wiadomości. 

Administratorzy globalni mogą również uruchomić polecenie [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , aby dowiedzieć się więcej o aktualnym stanie uaktualnienia.
