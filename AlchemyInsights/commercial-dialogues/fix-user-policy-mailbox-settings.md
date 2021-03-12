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
# <a name="fix-user-policymailbox-settings"></a>Naprawianie ustawień zasad użytkownika/skrzynki pocztowej

Ustawienia wiadomości-śmieci w skrzynce pocztowej mają wpływ na tę wiadomość. Aby przejrzeć ustawienia, wykonaj następujące czynności:

1. Uruchom powłokę zarządzania programu Exchange. Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programu Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Uruchom to polecenie (przy użyciu adresu e-mail użytkownika):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Sprawdź, czy adres e-mail nadawcy jest częścią **trustedSendersAndDomains** lub **BlockedSendersAndDomains.** Jeśli adres e-mail znajduje się na jednej z list, może być konieczne jego usunięcie. Aby dowiedzieć się więcej, [zobacz Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
