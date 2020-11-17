---
title: Tworzenie grupy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088910"
---
# <a name="create-a-group"></a>Tworzenie grupy

W tym temacie opisano tworzenie grup.

**Uprawnienie do tworzenia grupy**

Upewnij się, że masz autoryzację do tworzenia nowej grupy. Administratorzy globalni mogą wyłączyć tworzenie grup w witrynie Azure Portal lub panelu programu Access. Aby utworzyć nową grupę lub uzyskać odpowiednie uprawnienia, może być konieczne posiadanie administratora.

**Zarządzanie uprawnieniami do tworzenia grup**

1. Administratorzy globalni mogą zarządzać uprawnieniami do tworzenia grup (z powodów związanych z zabezpieczeniami) lub grup usługi Office 365 utworzonych w witrynie Azure Portal lub panelu dostępu, wybierając pozycję "użytkownicy mogą tworzyć grupy zabezpieczeń w portalu Azure" lub "użytkownicy mogą tworzyć grupy usługi Office 365 w obszarze portale Azure" — Opcje we **wszystkich grupach**—  >  **Ogólne (Ustawienia)**.
2. Możesz również ograniczyć możliwość tworzenia grup, aby wybrać grupę użytkowników, jeśli masz licencję usługi Azure Active Directory P1 Premium.

**Wyłączanie powiadomienia powitalnego dla nowych członków grupy pakietu Office 365**

Powiadomienie powitalne wysyłane do użytkowników, którzy są dodawani do grup usługi Office 365, można wyłączyć, ustawiając **UnifiedGroupWelcomeMessageEnabled** na false (FAŁSZ) w programie PowerShell. Dowiedz się więcej o [tym ustawieniu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

