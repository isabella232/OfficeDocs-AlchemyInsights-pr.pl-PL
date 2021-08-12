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
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940685"
---
# <a name="teams-add-in-for-mac"></a>Teams dla komputerów Mac

Aby rozwiązać problemy z brakującym Teams dla użytkowników systemu operacyjnego Mac, wykonaj następujące czynności:

**Krok 1.** Jeśli masz hybrydowe Exchange lokalne (wymagane jest 2016 CU3 lub nowsze), użyj narzędzia Test-HMA.ps1, aby potwierdzić, że nowoczesne uwierzytelnianie hybrydowe jest poprawnie skonfigurowane. Aby uzyskać więcej informacji, zobacz Konfigurowanie nowoczesnego uwierzytelniania na platformach [Outlook dla systemów iOS i Android.](https://aka.ms/TestHMAEAS)  

**Uwaga** Użyj formatu adresu UPN (na przykład [username@contoso.com](mailto:username@contoso.com)), a nie domena #D0 a nazwa_użytkownika. Robisz to nawet w przypadku użytkowników, Exchange Online skrzynki pocztowe.

**Krok 2.** Niech użytkownik może przejść do **narzędzia**  >  **Konta...** w Outlook dla komputerów Mac, a następnie znajdź i wybierz konto. Upewnij się, że wymieniona nazwa użytkownika ma format UPN (na [przykład username@contoso.com).](mailto:username@contoso.com)

**Krok 3.** Upewnij się, że użytkownik jest licencjonowanym Microsoft Teams użytkownikiem. Użytkownik musi korzystać z subskrypcji usługi Office 365 dla komputerów Mac w wersji produktu 16.24 lub nowszej.