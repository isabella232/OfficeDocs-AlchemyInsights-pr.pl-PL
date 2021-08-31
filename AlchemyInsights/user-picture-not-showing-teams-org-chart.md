---
title: Obraz użytkownika nie jest pokazywany na Microsoft Teams schematu organizacyjnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792761"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Obraz użytkownika nie jest pokazywany na Microsoft Teams schematu organizacyjnego

Jeśli zdjęcie profilowe danej osoby w organizacji nie jest wyświetlane na wykresie organizacyjnym, może to być możliwe, że ustawienie **ShowInAddressLists** ma wartość **False:**

1. Przejdź do centrum administracyjne platformy Microsoft 365 > [**Aktywni użytkownicy**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)i wybierz użytkownika z brakującym zdjęciem. 
1. Wybierz **kartę Poczta** i upewnij się, że ustawienie Pokaż **na globalnej liście adresowej** ma wartość **Tak.** 

Jeśli ustawienie **wartości ShowInAddressLists na** **Yes** (Tak) nie działa, sprawdź następujące kwestie:

- Użytkownik może być ukryty na liście adresatów w Exchange. Aby uzyskać więcej informacji, zobacz [Zarządzanie listami adresów w programie Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Użytkownik może być ukryty na liście adresów w Azure Active Directory. Aby uzyskać więcej informacji, [zobacz Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
