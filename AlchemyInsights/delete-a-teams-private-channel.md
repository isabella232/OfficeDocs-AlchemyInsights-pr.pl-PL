---
title: Usuwanie kanału prywatnego teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439919"
---
# <a name="delete-a-teams-private-channel"></a>Usuwanie kanału prywatnego teams

Firma Microsoft jest świadoma problemu z usunięciem kanału prywatnego usługi Teams, jeśli w podstawowej witrynie programu SharePoint włączono zasady przechowywania programu SharePoint. Firma Microsoft pracuje nad poprawką. W międzyczasie można użyć następujących obejść, aby usunąć kanał prywatny.

**Wyklucz zespół/zbiór witryn z zasad przechowywania programu Sharepoint.**

1. Przejdź do portalu administracyjnego usługi Office 365 i wybierz pozycję **Pokaż wszystko** w lewym okienku nawigacji.
2. W **obszarze Centra administracyjne**przejdź do pozycji Zasady zapobiegania utracie danych **dotyczących zgodności &**  >  **Data Loss Prevention**  >  **Policy**bezpieczeństwa .
3. Zidentyfikuj wszystkie zasady, które mają zastosowanie do witryn programu Sharepoint, i zmodyfikuj zasady, aby witryna programu SharePoint dla zespołu zawierającego kanał prywatny NIE została uwzględniona w zasadach przechowywania.
4. Zapisz zasady.
    Wprowadzanie ustawień zasad może potrwać do 24 godzin.
    Po wykluczeniu witryny można usunąć kanał prywatny.  
    
Możesz ***might*** usunąć kanał prywatny przy użyciu usługi Microsoft Teams na urządzeniu z systemem Android. 

Aby uzyskać powiązane informacje o programie SharePoint, zobacz [Nie można usunąć elementów w usłudze SharePoint Online lub usłudze OneDrive dla Firm](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).