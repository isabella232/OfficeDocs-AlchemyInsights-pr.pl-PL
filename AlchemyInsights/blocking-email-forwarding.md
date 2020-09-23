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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219865"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="71a4d-102">Blokowanie i odblokowywanie przekierowywania poczty e-mail</span><span class="sxs-lookup"><span data-stu-id="71a4d-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="71a4d-103">Aby włączyć lub wyłączyć przesyłanie dalej wiadomości e-mail dla konkretnej skrzynki pocztowej, zobacz [Konfigurowanie przekierowywania poczty e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="71a4d-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="71a4d-104">Po przeprowadzeniu kontroli nad przekazaniem zewnętrznym na poziomie dzierżawy jest używana zasada zapobiegania spamowi.</span><span class="sxs-lookup"><span data-stu-id="71a4d-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="71a4d-105">Jeśli to ustawienie jest wyłączone lub automatyczne, możesz zablokować przesyłanie poczty e-mail przy użyciu funkcji "550 5.7.520 Access odmowa dostępu, ponieważ organizacja nie zezwala na błąd w Twojej zewnętrznej przekierowaniu".</span><span class="sxs-lookup"><span data-stu-id="71a4d-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="71a4d-106">Następnie, jeśli przesyłanie dalej zostało ustawione jako zablokowane, to jest błąd widoczny dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="71a4d-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="71a4d-107">Jeśli przesyłanie dalej jest blokowane, upewnij się, że skonfigurowano zasady umożliwiające włączenie zewnętrznego autoprzekazywania.</span><span class="sxs-lookup"><span data-stu-id="71a4d-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="71a4d-108">Zasady filtrowania z wychodzącymi spamami można sprawdzić w centrum zabezpieczeń i zgodności albo przez uruchomienie polecenia Get-HostedOutboundSpamFilterPolicy | Nazwa FL, autoprzesyłanie dalej.</span><span class="sxs-lookup"><span data-stu-id="71a4d-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="71a4d-109">Jeśli chcesz skonfigurować blokowanie autoprzesyłania dalej, to samo polecenie poinformuje Cię o stanie zasad teraz.</span><span class="sxs-lookup"><span data-stu-id="71a4d-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="71a4d-110">Uwaga: zaleca się pozostawienie zewnętrznego autowiadomości bez wyłączenia na domyślnych zasadach filtrowania spamu dla połączeń wychodzących i włączenie tej funkcji tylko dla użytkowników wymagających przekierowania zewnętrznego przez utworzenie dla tych użytkowników zasad niestandardowych.</span><span class="sxs-lookup"><span data-stu-id="71a4d-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="71a4d-111">Aby dowiedzieć się więcej, zobacz [Konfigurowanie zewnętrznej obsługi przekierowywania wiadomości e-mail w pakiecie Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="71a4d-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>