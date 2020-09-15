---
title: Jak wyłączyć grupy zewnętrzne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704138"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="5dcc4-102">Jak wyłączyć grupy zewnętrzne</span><span class="sxs-lookup"><span data-stu-id="5dcc4-102">How to disable External Groups</span></span>

<span data-ttu-id="5dcc4-103">Komunikacja zewnętrzna usługi Yammer umożliwia stosowanie reguł transportu programu Exchange (ETR), zestawu aktywnych kontrolek w celu uniemożliwienia udostępniania informacji o firmie.</span><span class="sxs-lookup"><span data-stu-id="5dcc4-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="5dcc4-104">Aby uniemożliwić użytkownikom tworzenie grup zewnętrznych, należy skonfigurować regułę transportu programu Exchange (regułę), a następnie skonfigurować usługę Yammer do korzystania z reguły transportu programu Exchange w celu blokowania wiadomości zewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="5dcc4-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="5dcc4-105">Po utworzeniu reguły w centrum administracyjnym usługi Exchange Online wykonaj poniższe czynności, aby ustawić regułę do zastosowania w usłudze Yammer:</span><span class="sxs-lookup"><span data-stu-id="5dcc4-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="5dcc4-106">Zaloguj się do usługi Yammer jako zweryfikowany administrator, a następnie w **centrum administracyjnym usługi Yammer**przejdź do obszaru C \*\* \> Ustawienia zabezpieczeń zawartości i zabezpieczeń.\*\*</span><span class="sxs-lookup"><span data-stu-id="5dcc4-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="5dcc4-107">W obszarze **wiadomości zewnętrzne**wybierz pozycję **Wymuś reguły transportu usługi Exchange Online Exchange (ETR) w usłudze Yammer.**</span><span class="sxs-lookup"><span data-stu-id="5dcc4-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="5dcc4-108">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="5dcc4-108">Choose **Save**.</span></span>

<span data-ttu-id="5dcc4-109">Aby uzyskać więcej informacji, zobacz [wyłączanie wiadomości zewnętrznych w sieci Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="5dcc4-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  