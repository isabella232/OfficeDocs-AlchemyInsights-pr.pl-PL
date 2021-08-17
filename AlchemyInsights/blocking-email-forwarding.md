---
title: 726 Blokowanie przesyłania dalej wiadomości e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059642"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokowanie lub odblokowywanie przesyłania dalej wiadomości e-mail

Aby włączyć lub wyłączyć przesyłanie dalej wiadomości e-mail dla określonej skrzynki pocztowej, zobacz [Konfigurowanie przesyłania dalej poczty e-mail.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na poziomie dzierżawy kontrola nad zewnętrznym przesyłaniem dalej jest wykonywana przy użyciu zasad spamu ruchu wychodzącego. Zasady filtrowania spamu ruchu wychodzącego możesz sprawdzić tutaj w [Centrum](https://protection.office.com/antispam) zabezpieczeń i zgodności lub przy użyciu polecenia [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Jeśli jest wyświetlany następujący błąd: "Odmowa dostępu **550 5.7.520,** Twoja organizacja nie zezwala na przesyłanie dalej zewnętrzne", upewnij się, że zasady są skonfigurowane do włączania automatycznego przesyłania dalej zewnętrznego.

**Uwaga:** Zalecane jest, aby w domyślnych zasadach filtrowania spamu ruchu wychodzącego wyłączyć Autoforward zewnętrzny i włączyć tę funkcję tylko dla użytkowników, którzy potrzebują przesyłania dalej zewnętrznego, przez utworzenie zasad niestandardowych dla tych użytkowników. Aby uzyskać więcej informacji, [zobacz Konfigurowanie zewnętrznego przesyłania dalej poczty e-mail w programie Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)