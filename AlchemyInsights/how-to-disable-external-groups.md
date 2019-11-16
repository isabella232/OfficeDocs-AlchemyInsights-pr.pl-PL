---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739503"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4e34e-102">Jak wyłączyć grupy zewnętrzne</span><span class="sxs-lookup"><span data-stu-id="4e34e-102">How to disable External Groups</span></span>

<span data-ttu-id="4e34e-103">Yammer wiadomości zewnętrznych stosuje zasady transportu Exchange (ETRs), zestaw aktywnych formantów, aby zapobiec udostępnianiu informacji o firmie.</span><span class="sxs-lookup"><span data-stu-id="4e34e-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4e34e-104">Aby ograniczyć użytkownikom tworzenie grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (ETR), a następnie skonfigurować Yammer do używania reguły transportu programu Exchange do blokowania wiadomości zewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="4e34e-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4e34e-105">Po utworzeniu reguły w centrum administracyjnym programu Exchange Online, wykonaj następujące kroki, aby ustawić ETR do zastosowania w Yammer:</span><span class="sxs-lookup"><span data-stu-id="4e34e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4e34e-106">Zaloguj się do Yammer jako zweryfikowanego administratora, a w **centrum administracyjnym Yammer**przejdź do **zawartości C i ustawienia \> zabezpieczeń zabezpieczeń.**</span><span class="sxs-lookup"><span data-stu-id="4e34e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4e34e-107">W obszarze **wiadomości zewnętrznych**, wybierz opcję **Wymuszaj Exchange Online Exchange Transport Rules (ETRs) w Yammer.**</span><span class="sxs-lookup"><span data-stu-id="4e34e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4e34e-108">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="4e34e-108">Choose **Save**.</span></span>

<span data-ttu-id="4e34e-109">Aby uzyskać więcej informacji, zobacz [wyłączanie obsługi wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="4e34e-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  