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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929315"
---
# <a name="create-a-group"></a>Tworzenie grupy

W tym temacie opisano tworzenie grup.

**Uprawnienie do tworzenia grupy**

Upewnij się, że masz upoważnienie do tworzenia nowej grupy. Administratorzy globalni mogą wyłączyć tworzenie grup w Portalu Azure lub panelu dostępu. Administrator może utworzyć nową grupę lub nadać Ci odpowiednie uprawnienia.

**Zarządzanie uprawnieniami do tworzenia grup**

1. Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup (ze względów bezpieczeństwa) lub grupami programu Office 365 utworzonymi w Portalu Azure lub Panelu dostępu, wybierając opcję "Użytkownicy mogą tworzyć grupy zabezpieczeń w portalach Azure" lub "Użytkownicy mogą tworzyć grupy Office 365 w portalach Azure" w grupie Wszystkie grupy  >  **ogólne (Ustawienia).**
2. Możesz również ograniczyć tworzenie grup, aby wybrać grupę użytkowników, jeśli masz licencję grupy Azure Active Directory P1 Premium grupy.

**Wyłączanie powiadomień powitalnych dla nowych Office 365 członków grupy**

Powiadomienie powitalne wysyłane do użytkowników dodanych do grup Office 365 można wyłączyć, ustawiając wartość **UnifiedGroupWelcomeMessageEnabled na** False w programie PowerShell. Tutaj dowiesz się o tym [ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

