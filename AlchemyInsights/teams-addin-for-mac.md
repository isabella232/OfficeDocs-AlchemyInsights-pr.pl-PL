---
title: Dodatek Teams dla komputerów Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629771"
---
# <a name="teams-add-in-for-mac"></a>Dodatek Teams dla komputerów Mac

Aby rozwiązać problemy z brakującymi dodatkami dla użytkowników systemu operacyjnego dla komputerów Mac, wykonaj następujące czynności:

**Krok 1.** Jeśli masz lokalnie lokalny program Exchange (2016 CU3 lub nowszy), użyj narzędzia Test-HMA.ps1, aby upewnić się, że nowoczesne uwierzytelnianie hybrydowe jest poprawnie skonfigurowane. Aby uzyskać więcej informacji, zobacz [Sprawdzanie poprawności konfiguracji nowoczesnego uwierzytelniania dla aplikacji Outlook dla systemów iOS i Android](https://aka.ms/AA980zq).  

**Uwaga** Użyj formatu adresu UPN (na przykład [username@contoso.com](mailto:username@contoso.com)), a nie domena azwa_użytkownika. Zrób to nawet użytkownikom korzystającym ze skrzynek pocztowych usługi Exchange Online.

**Krok 2.** Użytkownik powinien przejść do **narzędzi**  >  **konta**... w programie Outlook dla komputerów Mac, a następnie Znajdź i zaznacz konto. Potwierdź, że nazwa użytkownika jest podana w formacie UPN (na przykład [username@contoso.com](mailto:username@contoso.com)).

**Krok 3:** Potwierdź, że użytkownik jest licencjonowanym użytkownikiem aplikacji Microsoft Teams. Użytkownik musi korzystać z subskrypcji pakietu Office 365 dla komputerów Mac, produktu w wersji 16,24 lub nowszej.