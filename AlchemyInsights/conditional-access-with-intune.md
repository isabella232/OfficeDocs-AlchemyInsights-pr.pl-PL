---
title: Dostęp warunkowy z usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931446"
---
# <a name="conditional-access-with-intune"></a>Dostęp warunkowy z usłudze Intune

Korzystanie z **dostępu warunkowego** z usłudze Intune wymaga 3 kroków:

- Utwórz **zasady zgodności** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne. Na przykład urządzenie musi mieć pin co najmniej 6 cyfr, zanim zostanie uznane za zgodne.
- Utwórz **zasady dostępu warunkowego,** który określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.  [Na przykład](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) urządzenie musi być zgodne przed dostępem do firmowej poczty e-mail.
- Upewnij się, że zarówno **zasady zgodności,** jak i **zasady dostępu warunkowego** są kierowane do pożądanych grup użytkowników. Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.

**Pomocne linki:**

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów z urzędem certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Aby chronić pocztę e-mail (Exchange online) przed dostępem przez niezgodne urządzenia, oba dokumenty muszą być przestrzegane:

1. [Ochrona dostępu do poczty e-mail przed urządzeniami za pomocą usługi EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrona dostępu do poczty e-mail przed urządzeniami przy użyciu nowoczesnych klientów uwierzytelniania, takich jak Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)