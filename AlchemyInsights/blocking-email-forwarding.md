---
title: 726 blokowanie przekierowywania poczty e-mail
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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473111"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="5511d-102">Blokowanie i odblokowywanie przekierowywania poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="5511d-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="5511d-103">Aby włączyć lub wyłączyć przesyłanie dalej wiadomości e-mail dla konkretnej skrzynki pocztowej, zobacz [Konfigurowanie przekierowywania poczty e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5511d-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="5511d-104">Po przeprowadzeniu kontroli nad przekazaniem zewnętrznym na poziomie dzierżawy jest używana zasada spamu.</span><span class="sxs-lookup"><span data-stu-id="5511d-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="5511d-105">Zasady filtrowania spamu wychodzącego można sprawdzić z Centrum zabezpieczeń i zgodności [tutaj] ( https://protection.office.com/antispam) lub za pomocą [polecenia Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="5511d-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="5511d-106">Jeśli jest wyświetlany następujący błąd: **"550 5.7.520 odmowa dostępu, Twoja organizacja nie zezwala na przekazanie zewnętrzne"**, upewnij się, że zasady są skonfigurowane do włączania automatycznego przekazywania zewnętrznego.</span><span class="sxs-lookup"><span data-stu-id="5511d-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="5511d-107">**Uwaga:** Zaleca się pozostawienie zewnętrznego autoprzesyłania dalej na domyślnych zasadach filtrowania spamu i włączenie tej funkcji tylko dla użytkowników wymagających przekierowania zewnętrznego przez utworzenie dla tych użytkowników zasad niestandardowych.</span><span class="sxs-lookup"><span data-stu-id="5511d-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="5511d-108">Aby dowiedzieć się więcej, zobacz [Konfigurowanie zewnętrznej obsługi przekierowywania wiadomości e-mail w pakiecie Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5511d-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>