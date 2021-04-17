---
title: Tworzenie grupy
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816367"
---
# <a name="create-a-group"></a>Tworzenie grupy

W tym temacie opisano tworzenie grup.

**Uprawnienie do tworzenia grupy**

Upewnij się, że masz upoważnienie do tworzenia nowej grupy. Administratorzy globalni mogą wyłączyć tworzenie grup w Portalu Azure lub panelu dostępu. Administrator może utworzyć nową grupę lub nadać Ci odpowiednie uprawnienia.

**Zarządzanie uprawnieniami do tworzenia grup**

1. Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup (ze względów bezpieczeństwa) lub grupami usługi Office 365 utworzonymi w Portalu Azure lub w Panelu dostępu, wybierając pozycję "Użytkownicy mogą tworzyć grupy zabezpieczeń w portalach Azure" lub "Użytkownicy mogą tworzyć grupy usługi Office 365 w portalach Azure" w grupie Wszystkie grupy ogólne  >  **(ustawienia).**
2. Jeśli masz licencję Usługi Azure Active Directory P1 Premium, możesz też ograniczyć tworzenie grup w celu wybrania grupy użytkowników.

**Wyłączanie powiadomień powitalnych dla nowych członków grupy usługi Office 365**

Powiadomienie powitalne wysyłane do użytkowników dodanych do grup usługi Office 365 można wyłączyć, ustawiając dla opcji **UnifiedGroupWelcomeMessageEnabled wartość False** w programie PowerShell. Tutaj dowiesz się o tym [ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

