---
title: Dostęp warunkowy w usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069722"
---
# <a name="conditional-access-with-intune"></a>Dostęp warunkowy w usłudze Intune

Korzystanie  **z dostępu warunkowego**  w usłudze Intune wymaga 3 kroków:

- Utwórz zasady **zgodności** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)w celu zdefiniowania ustawień, które muszą być spełnione, aby urządzenie zostało uznane za zgodne. Na przykład urządzenie musi mieć co najmniej 6-cyfrowy numer PIN, aby zostało uznane za zgodne.
- Utwórz zasady **dostępu warunkowego**  definiujące zasoby, które są chronione oraz wymagania, które należy spełnić, aby uzyskać do nich dostęp.  [Na przykład urządzenie musi](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  być zgodne, aby uzyskać dostęp do firmowej poczty e-mail.
- Upewnij **się, że zarówno**  zasady zgodności, jak i zasady dostępu  **warunkowego**  są kierowane do odpowiednich grup użytkowników. Może to wymagać utworzenia konkretnych grup użytkowników w Azure Active Directory.

**Przydatne linki:**

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów z urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Aby chronić pocztę e-Exchange online przed dostępem przez urządzenia nieuprawniane, należy przestrzegać obu dokumentów:

1. [Ochrona dostępu do poczty e-mail przed urządzeniami za pomocą eas](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrona dostępu do poczty e-mail przed urządzeniami za pomocą klientów nowoczesnego uwierzytelniania, takich jak Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)