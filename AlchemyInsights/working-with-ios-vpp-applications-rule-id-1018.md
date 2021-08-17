---
title: Praca z regułą VPP aplikacji systemu iOS o identyfikatorze 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083024"
---
# <a name="working-with-ios-vpp-applications"></a>Praca z aplikacjami VPP systemu iOS

Przeczytaj Jak zarządzać aplikacjami systemu iOS zakupionymi w ramach programu zakupu [volume-purchase](https://docs.microsoft.com/intune/vpp-apps-ios) wraz z aplikacją Microsoft Intune, aby dowiedzieć się więcej o funkcjach, ograniczeniach i krokach korzystania z programu zakupu licencjonowania głośność firmy Apple oraz o obsłudze tego programu w Microsoft Intune.
  
 **Typowe problemy:** "Aplikacja VPP systemu iOS została przypisana do moich użytkowników, ale instalacja nie powiodła się".
  
- Może się tak zdarzyć, jeśli jeden token VPP jest używany u wielu dostawców zarządzania urządzeniami przenośnymi. Tokeny VPP firmy Apple mogą być używane tylko u jednego dostawcy. Jeśli token VPP był używany u wielu dostawców, musisz go ponownie przekazać do usługi Intune.

- Instalacja może również się nie powieść, jeśli łączna liczba instalacji przekracza liczbę licencji. Aby wyświetlić raport użycia licencji, przejdź do strony licencji aplikacji **mobilnych Intune.** \>  Aby dowiedzieć się, jak odzyskać licencje w użyciu, zobacz [ten artykuł.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
