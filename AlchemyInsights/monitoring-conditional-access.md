---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702913"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorowanie dostępu warunkowego dla programu Exchange

Użytkownicy ukierunkowany na dostęp warunkowy otrzymają powiadomienie pocztą e-mail, jeśli nie spełnią wymagań organizacji dotyczących dostępu. W celu rozwiązania problemu zalecamy co najmniej jedno z następujących rozwiązań:
  
- Jeśli urządzenie jest uważane za zarejestrowane, zaleca się, aby użytkownik przeszedł do aplikacji Portal firmy i upewnić się, że jest wyświetlany w portalu firmy. Jeśli nie, użytkownik powinien zarejestrować urządzenie.
    
- W portalu Azure przejdź do obszaru usługi Intune dotyczącego ** \> zgodności**. W obszarze **monitor** kliknij pozycję **zgodność urządzenia**. Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne. 
    
- W portalu Azure przejdź do obszaru usługi Intune dotyczącego ** \> zgodności**. W obszarze **Zarządzanie**kliknij pozycję **zasady**. Na liście zasad zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli żaden profil nie jest przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia. 
    
- Edytowanie przydziału dostępu warunkowego użytkownika.
    
1. W portalu Azure Portal przejdź do ** \> \> zasad dostępu warunkowego usługi Intune**
    
2. Wybierz zasadę z listy
    
3. Kliknij pozycję **Użytkownicy i grupy**
    
4. Aby określić zasady jako docelowe dla określonej osoby, Dodaj je do listy **dołączania** . Aby upewnić się, że dana osoba zostanie pominięta w zasadach, Dodaj je do listy **wykluczania** . 
    
Dowiedz się więcej: [Jak monitorować urządzenia z dostępem warunkowym](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

