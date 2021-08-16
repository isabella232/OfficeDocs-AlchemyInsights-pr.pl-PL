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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034728"
---
# <a name="fix-user-policymailbox-settings"></a>Naprawianie ustawień zasad użytkownika/skrzynki pocztowej

Ustawienia wiadomości-śmieci w skrzynce pocztowej mają wpływ na tę wiadomość. Aby przejrzeć ustawienia, wykonaj następujące czynności:

1. Uruchom Exchange zarządzania. Aby uzyskać więcej informacji, [zobacz Otwieranie Exchange zarządzania danymi.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Uruchom to polecenie (przy użyciu adresu e-mail użytkownika):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Sprawdź, czy adres e-mail nadawcy jest częścią **trustedSendersAndDomains** lub **BlockedSendersAndDomains.** Jeśli adres e-mail znajduje się na jednej z list, może być konieczne jego usunięcie. Aby dowiedzieć się więcej, [zobacz Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
