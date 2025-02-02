---
title: Blokowanie lub odblokowywanie automatycznego przesyłania dalej zewnętrznych wiadomości e-mail
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315884"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokowanie lub odblokowywanie automatycznego przesyłania dalej wiadomości e-mail

Aby włączyć lub wyłączyć przesyłanie dalej wiadomości e-mail dla określonej skrzynki pocztowej, zobacz [Konfigurowanie przesyłania dalej poczty e-mail.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administratorzy mogą kontrolować zewnętrzne przesyłanie dalej w organizacji przy użyciu zasad [spamu wychodzącego.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Zasadami spamu ruchu wychodzącego można zarządzać w portalu usługi Microsoft 365 Defender w programie Exchange Online Shell lub przy użyciu polecenia <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Jeśli zostanie wyświetlony następujący błąd: "Odmowa dostępu **550 5.7.520,** Twoja organizacja nie zezwala na przesyłanie dalej zewnętrzne", upewnij się, że zasady są skonfigurowane tak, aby włączyć automatyczne przesyłanie dalej zewnętrznych wiadomości.

**Uwaga:** Zaleca się używanie wartości domyślnej  Automatycznie — **system** kontrolowany dla ustawienia Reguły automatycznego przesyłania dalej w domyślnych zasadach filtru spamu ruchu wychodzącego (automatyczne przekazywanie zewnętrzne jest zablokowane, wewnętrzne automatyczne przesyłanie dalej nadal działa). Należy utworzyć niestandardowe zasady filtrowania spamu ruchu wychodzącego i użyć wartości **Włączone —** funkcja przesyłania dalej jest włączona tylko dla użytkowników, którzy potrzebują automatycznego przesyłania dalej zewnętrznych wiadomości e-mail. Aby uzyskać więcej informacji, zobacz Konfigurowanie zewnętrznego przesyłania [dalej poczty e-mail w programie Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
