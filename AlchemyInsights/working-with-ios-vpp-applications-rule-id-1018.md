---
title: Praca z iOS 1018 identyfikator reguły aplikacji VPP
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364871"
---
# <a name="working-with-ios-vpp-applications"></a>Praca z iOS aplikacje VPP

Przeczytaj, [jak zarządzać aplikacje iOS kupione za pośrednictwem programu zakupu woluminu z usługi Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) Dowiedz się więcej o cechy, ograniczenia i czynności, aby poprawić wykorzystanie programu zakupu zbiorowego Apple i wsparcie dla niego w Microsoft Intune.
  
 **Typowych problemów:** "Aplikacja VPP iOS przypisane do moich użytkowników, ale instalacja nie powiodła się".
  
- Może się to zdarzyć, jeśli pojedynczy token VPP jest używana na wielu dostawców zarządzania urządzenia przenośnego. Tokeny VPP, Apple może służyć wyłącznie u jednego dostawcy. Jeśli użyto VPP token z wieloma dostawcami, możesz ponownie przesłać token Windows Intune.

- Instalacja może się nie udać, jeśli całkowita ilość instalacji przekracza liczbę licencji. Aby wyświetlić raport użycia dla swoich licencji, przejdź do strony **Windows Intune aplikacje** \> strony **licencji aplikacji** . Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [w tym artykule.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
