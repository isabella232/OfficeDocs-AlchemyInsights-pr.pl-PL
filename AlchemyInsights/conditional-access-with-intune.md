---
title: Dostęp warunkowy za pomocą usługi Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807669"
---
# <a name="conditional-access-with-intune"></a>Dostęp warunkowy za pomocą usługi Intune

Używanie funkcji  **dostęp warunkowy**  z usługą Intune wymaga wykonania 3 kroków:

- Utwórz  **zasady zgodności**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne. Na przykład urządzenie musi mieć numer PIN o co najmniej 6 cyfrach, zanim zostanie uznany za zgodny.
- Utwórz **zasady dostępu warunkowego**  określające, jakie zasoby są chronione, a jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.  [Na przykład](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  urządzenie musi być zgodne przed uzyskaniem dostępu do firmowej poczty e-mail.
- Upewnij się, że **zasady zgodności**  i  **zasady dostępu warunkowego**  są kierowane do żądanych grup użytkowników. Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.

**Pomocne linki:**

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów dotyczących urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Aby chronić wiadomości E-mail (usługi Exchange Online) przed dostępem za pomocą urządzeń niezgodnych, muszą być stosowane oba dokumenty:

1. [Ochrona dostępu do poczty e-mail za pomocą urządzeń przy użyciu aplikacji EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrona dostępu do poczty e-mail za pomocą urządzeń przy użyciu nowoczesnych klientów uwierzytelniania, takich jak program Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)