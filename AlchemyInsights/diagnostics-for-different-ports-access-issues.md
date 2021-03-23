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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035777"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="b677d-102">Diagnostyka problemów z dostępem do różnych portów</span><span class="sxs-lookup"><span data-stu-id="b677d-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="b677d-103">Aby rozwiązać różne problemy z dostępem do portu, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="b677d-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="b677d-104">Zatrzymaj/deallocate maszyny wirtualnej z portalu, uruchom ponownie maszyny wirtualnej i ponownie przetestuj maszyny wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="b677d-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="b677d-105">Sprawdź ustawienia sieci maszyny wirtualnej, aby ustalić, czy masz grupy zabezpieczeń sieci blokujące ruch.</span><span class="sxs-lookup"><span data-stu-id="b677d-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="b677d-106">Za pomocą narzędzia do weryfikowania przepływu IP usługi [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) możesz również sprawdzić, czy grupy NSG nie blokują ruchu, User-Defined Trasy (UDR) przekierowywują ruch z powrotem do lokalnego ('Trasy domyślne' 0.0.0.0/0) lub do urządzenia sieciowego.</span><span class="sxs-lookup"><span data-stu-id="b677d-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="b677d-107">Jeśli nadal masz problemy po wypróbowaniu powyższych kroków, podaj nazwę maszyny wirtualnej i port TCP, przy użyciu których próbujesz wysłać pocztę w celu dalszej diagnozy.</span><span class="sxs-lookup"><span data-stu-id="b677d-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="b677d-108">**Polecane dokumenty**</span><span class="sxs-lookup"><span data-stu-id="b677d-108">**Recommended Documents**</span></span>

[<span data-ttu-id="b677d-109">Ograniczenia i zalecenia dotyczące wysyłania wychodzących wiadomości e-mail za pośrednictwem portu 25</span><span class="sxs-lookup"><span data-stu-id="b677d-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)