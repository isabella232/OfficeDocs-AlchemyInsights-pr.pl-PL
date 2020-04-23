---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720778"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="956e6-102">Jak wyłączyć grupy zewnętrzne</span><span class="sxs-lookup"><span data-stu-id="956e6-102">How to disable External Groups</span></span>

<span data-ttu-id="956e6-103">Usługa Yammer wiadomości zewnętrzne stosuje Exchange Transport Rules (ETRs), zestaw proaktywnych kontroli, aby zapobiec udostępnianiu informacji o firmie.</span><span class="sxs-lookup"><span data-stu-id="956e6-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="956e6-104">Aby ograniczyć użytkownikom możliwość tworzenia grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (ETR), a następnie skonfigurować usługę Yammer do blokowania obsługi wiadomości zewnętrznych za pomocą reguły transportu programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="956e6-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="956e6-105">Po utworzeniu reguły w centrum administracyjnym usługi Exchange Online wykonaj następujące kroki, aby ustawić etr do zastosowania w usłudze Yammer:</span><span class="sxs-lookup"><span data-stu-id="956e6-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="956e6-106">Zaloguj się do usługi Yammer jako zweryfikowany administrator, a następnie w **centrum administracyjnym usługi Yammer**przejdź do sekcji \*\*Ustawienia zawartości i zabezpieczeń C. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="956e6-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="956e6-107">W obszarze **Wiadomości zewnętrzne**wybierz pozycję **Wymuszaj reguły transportu wymiany online (ETR) w usłudze Yammer.**</span><span class="sxs-lookup"><span data-stu-id="956e6-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="956e6-108">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="956e6-108">Choose **Save**.</span></span>

<span data-ttu-id="956e6-109">Aby uzyskać więcej informacji, zobacz [Wyłączanie wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="956e6-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  