---
title: Identyfikator reguły aplikacji VPP systemu iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719967"
---
# <a name="working-with-ios-vpp-applications"></a>Praca z aplikacjami VPP na iOS

Przeczytaj [jak zarządzać aplikacjami na iOS zakupionymi za pośrednictwem programu zakupu zbiorczego w usłudze Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) aby dowiedzieć się więcej o funkcjach, ograniczeniach i krokach ułatwiania korzystania z programu zakupów zbiorczych Firmy Apple i obsługi technicznej w usłudze Microsoft Intune.
  
 **Typowe problemy:** "Przypisano aplikację VPP dla systemu iOS do moich użytkowników, ale instalacja nie powiodła się."
  
- Może się tak zdarzyć, jeśli pojedynczy token VPP jest używany przez wielu dostawców zarządzania urządzeniami przenośnymi. Tokeny VPP firmy Apple mogą być używane tylko z jednym dostawcą. Jeśli użyto tokenu VPP z wieloma dostawcami, należy ponownie przekazać token do usługi Intune.

- Instalacja może również zakończyć się niepowodzeniem, jeśli całkowita liczba instalacji przekroczy liczbę licencji. Aby wyświetlić raport użycia licencji, przejdź do strony **Licencje** **aplikacji aplikacji intune mobile.** \> Aby dowiedzieć się, jak odzyskać używane licencje, zobacz [ten artykuł.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
