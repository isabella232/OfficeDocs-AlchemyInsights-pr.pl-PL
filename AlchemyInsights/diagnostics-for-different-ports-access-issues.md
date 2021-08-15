---
title: Diagnostyka problemów z dostępem do różnych portów
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030912"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostyka problemów z dostępem do różnych portów

Aby rozwiązać różne problemy z dostępem do portu, wykonaj następujące czynności:

1. Zatrzymaj/deallocate maszyny wirtualnej z portalu, uruchom ponownie maszyny wirtualnej i ponownie przetestuj maszyny wirtualnej. 
2. Sprawdź ustawienia sieci maszyny wirtualnej, aby ustalić, czy masz grupy zabezpieczeń sieci blokujące ruch. Za pomocą narzędzia do weryfikowania przepływu IP usługi [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) możesz również sprawdzić, czy grupy NSG nie blokują ruchu, User-Defined Trasy (UDR) przekierowywują ruch z powrotem do lokalnego ('Trasy domyślne' 0.0.0.0/0) lub do urządzenia sieciowego.
Jeśli nadal masz problemy po wypróbowaniu powyższych kroków, podaj nazwę maszyny wirtualnej i port TCP, przy użyciu których próbujesz wysłać pocztę w celu dalszej diagnozy.

**Zalecane dokumenty**

[Ograniczenia i zalecenia dotyczące wysyłania wychodzących wiadomości e-mail za pośrednictwem portu 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)