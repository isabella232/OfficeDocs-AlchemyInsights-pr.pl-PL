---
title: Konfigurowanie szyfrowania wiadomości dla środowiska hybrydowego
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747953"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="f29c5-102">Konfigurowanie szyfrowania wiadomości dla środowiska hybrydowego</span><span class="sxs-lookup"><span data-stu-id="f29c5-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="f29c5-103">W przypadku hybrydowych środowisk programu Exchange lokalni użytkownicy mogą wysyłać zaszyfrowane wiadomości e-mail przy użyciu szyfrowania wiadomości pakietu Office (OME, Office Message Encryption) tylko wtedy, gdy wiadomości e-mail są kierowane za pośrednictwem usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f29c5-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="f29c5-104">Aby szyfrować wiadomości e-mail przy użyciu narzędzia OME, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="f29c5-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="f29c5-105">Skonfiguruj środowisko [hybrydowe za](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) pomocą Kreatora konfiguracji hybrydowej.</span><span class="sxs-lookup"><span data-stu-id="f29c5-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="f29c5-106">Do skonfigurowania szyfrowania nie są wymagane żadne specjalne kroki.</span><span class="sxs-lookup"><span data-stu-id="f29c5-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="f29c5-107">[Skonfiguruj reguły przepływu poczty e-mail w taki sposób, jak](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) zwykle.</span><span class="sxs-lookup"><span data-stu-id="f29c5-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


