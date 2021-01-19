---
title: Kontroler domeny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901309"
---
# <a name="domain-controller"></a>Kontroler domeny

**Nie można włączyć usługi AAD — w usłudze domenowych lub rozmieszczeniu jest niepowodzenie**

Aby rozwiązać problem z usługą domenowych w usłudze Azure AD (AAD-DS), która nie jest włączona lub nie ma zostać wdrożona, wykonaj następujące czynności:

1. Jeśli używasz już istniejącej sieci wirtualnej, zapoznaj się z NSG, aby uzyskać reguły blokujące porty potrzebne do synchronizacji w usłudze AAD-DS w portalu https://aka.ms/aadds-networking .
2. Sprawdź, czy w tym przewodniku podczas rozwiązywania problemów jest dostępny komunikat o błędzie  https://aka.ms/aadds-troubleshoot-enable .
3. Spróbuj wdrożyć usługi domenowe w usłudze Azure AD w nowej sieci wirtualnej.
4. Postępuj zgodnie z instrukcjami dotyczącymi wdrażania usługi AAD-DS, która jest dostępna w [samouczku dotyczącego tworzenia usług domenowych w usłudze Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jeśli masz problemy z wdrażaniem usług domenowych w usłudze Azure AD, zobacz [Rozwiązywanie problemów z usługami domenowymi usługi Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , aby rozwiązać typowe błędy ułatwiające ponowne rozpoczęcie pracy. 

**Nie można wyłączyć usługi AAD — DS**

Nie można wstrzymać usługi AAD — DS. Jeśli chcesz zatrzymać korzystanie z domeny zarządzanej, należy ją usunąć.

Jeśli występują problemy, aby rozwiązać typowe komunikaty o błędach i skojarzone kroki rozwiązywania problemów ułatwiające ponowne uruchomienie uruchamiania, zobacz [Rozwiązywanie problemów z usługami domenowymi Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
