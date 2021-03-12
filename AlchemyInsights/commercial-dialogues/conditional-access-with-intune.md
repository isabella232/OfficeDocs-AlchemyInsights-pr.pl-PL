---
title: Korzystanie z dostępu warunkowego w usłudze Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749258"
---
# <a name="using-conditional-access-with-intune"></a>Korzystanie z dostępu warunkowego w usłudze Intune

Korzystanie z dostępu warunkowego w usłudze Intune wymaga 3 kroków:

- [Utwórz zasady zgodności, aby zdefiniować ustawienia, które muszą być spełnione, aby urządzenie zostało uznane za zgodne. Na przykład urządzenie musi mieć co najmniej 6-cyfrowy numer PIN, aby zostało uznane za zgodne.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Utwórz zasady dostępu warunkowego definiujące zasoby, które są chronione oraz wymagania, które należy spełnić, aby uzyskać do nich dostęp. Na przykład urządzenie musi być zgodne, aby uzyskać dostęp do firmowej poczty e-mail.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Upewnij się, że zarówno zasady zgodności, jak i zasady dostępu warunkowego są kierowane do odpowiednich grup użytkowników. Może to wymagać utworzenia konkretnych grup użytkowników w usłudze Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Przeczytaj więcej...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
