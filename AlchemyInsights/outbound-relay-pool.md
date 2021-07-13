---
title: Pula przekazywania połączeń wychodzących
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381857"
---
# <a name="outbound-relay-pool"></a>Pula przekazywania połączeń wychodzących

Firma Microsoft wprowadza pewne zmiany w konfiguracji przekazywania lub przesyłania dalej poczty e-mail za pośrednictwem Microsoft 365. Wiadomości w określonych scenariuszach są przekazywane dalej lub przekazywane przez Microsoft 365 przy użyciu specjalnej puli przekazywania. Wiadomości wysłane przy użyciu puli przekazywania mogą trafiać do folderu wiadomości-śmieci adresata. Aby uzyskać więcej informacji, zobacz [Pule dostarczania połączeń wychodzących](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Aby uniknąć sytuacji używającej puli przekazywania, upewnij się, że wiadomości przekazane/przekazane spełniają jedno z następujących kryteriów:

- Nadawca ruchu wychodzącego jest zaakceptowaną domeną dzierżawy.
- Spf (Sender Policy Framework) przechodzi, gdy przychodzi wiadomość do Microsoft 365.
- DKIM (DomainKeys Identified Mail) w domenie nadawcy P2 przechodzi, gdy przychodzi wiadomość do Microsoft 365.
 
Wiadomości spełniające powyższe kryteria nie są przekazywane przez pulę przekazywania.

Jeśli rekord MX domeny wskazuje serwer innej firmy lub serwer lokalne, użyj funkcji rozszerzonego filtrowania, aby upewnić się, że weryfikacja SPF jest prawidłowa dla przychodzącej poczty e-mail i aby uniknąć wysyłania wiadomości e-mail za pośrednictwem puli przekazywania.

**Jak możemy stwierdzić, czy na nas wpływa pula przekazywania?**

Jeśli w przesyłanych lub przesyłanych wiadomościach e-mail jest stosowane jedno z powyższych kryteriów, wiadomości nie będą przekazywane przez pulę przekazywania. Jeśli jednak wiadomość jest wysyłana za pośrednictwem puli przekazywania, adres IP serwera ruchu wychodzącego należy do zakresu 40.95.0.0/16, a nazwa serwera ruchu wychodzącego zawiera nazwę **rly.**

