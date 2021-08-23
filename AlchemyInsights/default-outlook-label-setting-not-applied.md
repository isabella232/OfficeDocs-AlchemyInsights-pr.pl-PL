---
title: Domyślne Outlook etykiety nieuplikowane
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455091"
---
# <a name="default-outlook-label-setting-not-applied"></a>Domyślne Outlook etykiety nieuplikowane

Jeśli domyślne ustawienia etykiety programu Outlook nie działają poprawnie i zastosowano inną etykietę lub nie zastosowano żadnej etykiety, może to oznaczać, że występuje znany problem (MC277818) i należy wykonać jedną z tych 2 opcji, aby rozwiązać ten problem:

**Opcja 1.**

1. Przejdź do Microsoft 365 zgodności i > **informacji o**  >  **rozwiązaniach.**
1. Wybierz **pozycję Zasady** etykiet , a następnie wybierz zasady etykiet, które chcesz edytować (ustawienie **OutlookDefaultlabel** nie jest skonfigurowane poprawnie dla określonych zasad etykiet). Uruchom **polecenie Get-labelpolicy,** aby wyświetlić to ustawienie), a następnie wybierz **pozycję Edytuj zasady**.
1. Wybierz **pozycję Dalej,** aż zobaczysz ustawienie Zastosuj tę etykietę  domyślną do wiadomości e-mail, które jest dostępne, jeśli wybierzesz pozycję Wymagaj od użytkowników stosowania etykiety do wiadomości e-mail i dokumentów spadku w oknie dialogowym **Ustawienia** zasad. 
1. W **oknie dialogowym Stosowanie etykiety** domyślnej do dokumentów wybierz pozycję **Brak** z listy rozwijanej.
1. Wybierz **pozycję Dalej** i **Prześlij,** aby zapisać ustawienia etykiet.

**Opcja 2:**

W [programie PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)w Centrum zabezpieczeń i zgodności użyj polecenia Set-LabelPolicy, aby zmienić pozycję **OutlookDefaultlabel na** **Brak** na stronie {OutlookDefaultLabel="None"}.

Uruchamianie: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Aby uzyskać więcej informacji na temat etykiet Outlook etykiet, zobacz [Ustawianie innej etykiety](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)domyślnej dla etykiety Outlook.