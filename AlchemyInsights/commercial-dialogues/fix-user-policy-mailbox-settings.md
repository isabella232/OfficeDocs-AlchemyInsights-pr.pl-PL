---
title: Naprawianie ustawień zasad użytkownika/skrzynki pocztowej
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
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750558"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="57c7c-102">Naprawianie ustawień zasad użytkownika/skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="57c7c-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="57c7c-103">Ustawienia wiadomości-śmieci w skrzynce pocztowej mają wpływ na tę wiadomość.</span><span class="sxs-lookup"><span data-stu-id="57c7c-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="57c7c-104">Aby przejrzeć ustawienia, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="57c7c-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="57c7c-105">Uruchom powłokę zarządzania programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="57c7c-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="57c7c-106">Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programu Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="57c7c-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="57c7c-107">Uruchom to polecenie (przy użyciu adresu e-mail użytkownika):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="57c7c-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="57c7c-108">Sprawdź, czy adres e-mail nadawcy jest częścią **trustedSendersAndDomains** lub **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="57c7c-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="57c7c-109">Jeśli adres e-mail znajduje się na jednej z list, może być konieczne jego usunięcie.</span><span class="sxs-lookup"><span data-stu-id="57c7c-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="57c7c-110">Aby dowiedzieć się więcej, [zobacz Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="57c7c-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
