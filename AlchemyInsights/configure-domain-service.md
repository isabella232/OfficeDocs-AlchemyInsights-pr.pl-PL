---
title: Konfigurowanie usługi domeny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885692"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nie można włączyć usługi AAD — w usłudze domenowych lub rozmieszczeniu jest niepowodzenie

Aby rozwiązać problem z usługą domenowych w usłudze Azure AD (AAD-DS), która nie jest włączona lub nie ma zostać wdrożona, wykonaj następujące czynności:

1. Jeśli używasz już istniejącej sieci wirtualnej, zapoznaj się z NSG, aby uzyskać reguły blokujące porty potrzebne do synchronizacji w usłudze AAD-DS w portalu https://aka.ms/aadds-networking .
2. Sprawdź, czy w tym przewodniku podczas rozwiązywania problemów jest dostępny komunikat o błędzie  https://aka.ms/aadds-troubleshoot-enable .
3. Spróbuj wdrożyć usługi domenowe w usłudze Azure AD w nowej sieci wirtualnej.
4. Postępuj zgodnie z przewodnikiem wprowadzenie dotyczącym wdrażania usługi AAD — DS: [Tworzenie i Konfigurowanie usług domenowych w usłudze AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jeśli masz problemy z wdrażaniem usług domenowych w usłudze Azure AD, zobacz [Rozwiązywanie problemów z usługami domenowymi usługi Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , aby rozwiązać typowe błędy ułatwiające ponowne rozpoczęcie pracy. 

**Nie można wyłączyć usługi AAD — DS**

Nie można wstrzymać usługi AAD — DS. Jeśli chcesz zatrzymać korzystanie z domeny zarządzanej, należy ją usunąć.
Aby usunąć domenę zarządzaną, zobacz [usuwanie usługi domeny AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



