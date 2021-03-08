---
title: Konfigurowanie szyfrowania wiadomości w środowisku hybrydowym
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526597"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>Konfigurowanie szyfrowania wiadomości w środowisku hybrydowym

W przypadku hybrydowych środowisk programu Exchange lokalni użytkownicy mogą wysyłać zaszyfrowane wiadomości e-mail przy użyciu szyfrowania wiadomości pakietu Office (OME, Office Message Encryption) tylko wtedy, gdy wiadomości e-mail są kierowane za pośrednictwem usługi Exchange Online.

Aby zaszyfrować wiadomości e-mail przy użyciu narzędzia OME, wykonaj następujące czynności:

1. Skonfiguruj środowisko [hybrydowe za](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) pomocą Kreatora konfiguracji hybrydowej. W celu skonfigurowania szyfrowania nie są wymagane żadne specjalne kroki.
2. [Skonfiguruj reguły przepływu poczty e-mail do szyfrowania](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) tak jak zwykle.


