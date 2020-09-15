---
title: Praca z regułami aplikacji VPP dla systemu iOS o identyfikatorze 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688956"
---
# <a name="working-with-ios-vpp-applications"></a>Praca z aplikacjami VPP systemu iOS

W tym artykule [opisano, jak zarządzać aplikacjami z systemem iOS zakupionymi za pośrednictwem programu Volume Purchase Program z usługą Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , aby uzyskać informacje o funkcjach, ograniczeniach i krokach w celu skorzystania z programu Apple Volume Purchase i pomocy technicznej dla usługi Microsoft Intune.
  
 **Typowe problemy:** "Przypisano Ci aplikację VPP systemu iOS do użytkowników, ale instalacja nie powiodła się".
  
- Może się tak zdarzyć, jeśli jeden token VPP jest wykorzystywany przez wielu dostawców zarządzania urządzeniami przenośnymi. Tokeny VPP firmy Apple mogą być używane tylko z jednym dostawcą. Jeśli korzystasz z tokenu VPP z wieloma dostawcami, musisz ponownie przekazać token do usługi Intune.

- Instalacja może również zakończyć się niepowodzeniem, jeśli łączna liczba instalacji przekracza liczbę licencji. Aby wyświetlić raport użycia licencji, przejdź do **Intune Mobile apps** \> strony **licencje aplikacji** usługi Intune dla urządzeń przenośnych. Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [ten artykuł.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
