---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713728"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorowanie dostępu warunkowego dla programu Exchange

Użytkownicy objęci dostępem warunkowym otrzymają wiadomość e-mail z powiadomieniem, jeśli nie spełniają wymagań dotyczących dostępu w organizacji. Aby rozwiązać problem, zaleca się co najmniej jedno z następujących rozwiązań:
  
- Jeśli zakłada się, że urządzenie jest zarejestrowane, poinformuj go o tym, aby przejść do aplikacji Portal firmy i sprawdzić, czy jest ono wyświetlane w portalu firmy. Jeśli tak nie jest, użytkownik powinien zarejestrować urządzenie.
    
- W witrynie Azure portal przejdź do **zgodności urządzenia usługi Intune \> **. W obszarze **Monitor kliknij** pozycję **Zgodność urządzenia**. Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne. 
    
- W witrynie Azure portal przejdź do **zgodności urządzenia usługi Intune \> **. W obszarze **Zarządzanie**kliknij pozycję **Zasady**. Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli nie zostanie przypisany żaden profil, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia. 
    
- Edytuj przypisanie dostępu warunkowego użytkownika.
    
1. W witrynie Azure Portal przejdź do **zasad dostępu \> \> warunkowego usługi Intune**
    
2. Wybieranie zasad z listy
    
3. Kliknij **pozycję Użytkownicy i grupy**
    
4. Aby skierować do innej osoby określone zasady, dodaj je do listy **Dołącz.** Aby upewnić się, że dana osoba została pominięta w zasadach, dodaj ją do listy **Wyklucz.** 
    
Czytaj więcej: [Jak monitorować urządzenia dostępu warunkowego](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

