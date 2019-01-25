---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482443"
---
# <a name="monitoring-conditional-access"></a>Monitorowanie dostępu warunkowego

Użytkownicy kierowana do dostępu warunkowego otrzymają wiadomość e-mail z powiadomieniem, jeżeli nie spełniają one wymagań dostępu organizacji. Aby rozwiązać, zaleca się jeden lub kilka z następujących rozwiązań:
  
- W przypadku przyjmuje się, że urządzenie się zarejestrować, należy poinformować użytkownika, aby przejść do aplikacji Portal firmy i sprawdź, czy pojawia się w portalu firmy. Jeśli tak nie jest, użytkownik należy zarejestrować urządzenia.
    
- W portalu Azure przejdź do **Intune \> zgodności urządzenia**. W obszarze **monitora** kliknij **zgodności urządzenia**. Wyświetlanie raportu zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczony jako zgodny z. 
    
- W portalu Azure przejdź do **Intune \> zgodności urządzenia**. W obszarze **Zarządzaj**kliknij **zasady**. Na liście zasady zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeżeli żaden profil nie jest przypisany, Intune nie będzie mógł potwierdzić stan zgodności urządzenia. 
    
- Edytuj przypisanie warunkowego dostępu użytkownika.
    
1. W portalu Azure przejdź do **Intune \> dostępu warunkowego \> zasady**
    
2. Wybierz zasadę z listy
    
3. Kliknij przycisk **Użytkownicy i grupy**
    
4. Aby skierować pewną politykę na kogoś, należy dodać je do listy **dołączania** . W celu zapewnienia, że osoba zostanie pominięty, z zasady, należy dodać je do listy **wykluczeń** . 
    
Przeczytaj więcej: [jak urządzeń dostępu warunkowego monitora](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

