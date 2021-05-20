---
title: Teams dla komputerów Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582080"
---
# <a name="teams-add-in-for-mac"></a>Teams dla komputerów Mac

Aby rozwiązać problemy z brakującym Teams dla użytkowników systemu operacyjnego Mac, wykonaj następujące czynności:

**Krok 1.** Jeśli masz hybrydowe Exchange lokalne (wymagane jest 2016 CU3 lub nowsze), użyj narzędzia Test-HMA.ps1, aby potwierdzić, że nowoczesne uwierzytelnianie hybrydowe jest poprawnie skonfigurowane. Aby uzyskać więcej informacji, zobacz Konfigurowanie nowoczesnego uwierzytelniania na platformach [Outlook dla systemów iOS i Android.](https://aka.ms/TestHMAEAS)  

**Uwaga** Użyj formatu adresu UPN (na przykład [username@contoso.com](mailto:username@contoso.com)), a nie domena #D0 a nazwa_użytkownika. Robisz to nawet w przypadku użytkowników, Exchange Online skrzynki pocztowe.

**Krok 2.** Niech użytkownik może przejść do **narzędzia**  >  **Konta...** w Outlook dla komputerów Mac, a następnie znajdź i wybierz konto. Upewnij się, że wymieniona nazwa użytkownika ma format UPN (na [przykład username@contoso.com).](mailto:username@contoso.com)

**Krok 3.** Upewnij się, że użytkownik jest licencjonowanym Microsoft Teams użytkownikiem. Użytkownik musi korzystać z subskrypcji usługi Office 365 dla komputerów Mac w wersji produktu 16.24 lub nowszej.