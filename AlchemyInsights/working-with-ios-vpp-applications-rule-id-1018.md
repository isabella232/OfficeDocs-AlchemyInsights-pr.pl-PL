---
title: Praca z iOS 1018 identyfikator reguły aplikacji VPP
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483063"
---
# <a name="working-with-ios-vpp-applications"></a>Praca z iOS aplikacje VPP

Przeczytaj, [jak zarządzać aplikacje iOS kupione za pośrednictwem programu zakupu woluminu z usługi Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) Dowiedz się więcej o cechy, ograniczenia i czynności, aby poprawić wykorzystanie programu zakupu zbiorowego Apple i wsparcie dla niego w Microsoft Intune. 
  
 **Typowych problemów:** "Aplikacja VPP iOS przypisane do moich użytkowników, ale instalacja nie powiodła się". 
  
- Może się to zdarzyć, jeśli pojedynczy token VPP jest używana na wielu dostawców zarządzania urządzenia przenośnego. Tokeny VPP, Apple może służyć wyłącznie u jednego dostawcy. Jeśli użyto VPP token z wieloma dostawcami, możesz ponownie przesłać token Windows Intune.
    
- Instalacja może się nie udać, jeśli całkowita ilość instalacji przekracza liczbę licencji. Aby wyświetlić raport użycia dla swoich licencji, przejdź do strony **Windows Intune aplikacje** \> strony **licencji aplikacji** . Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [w tym artykule.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

