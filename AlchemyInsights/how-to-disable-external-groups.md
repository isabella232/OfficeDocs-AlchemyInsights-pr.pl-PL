---
title: Jak wyłączyć grup zewnętrznych
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399673"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="f31a2-102">Jak wyłączyć grup zewnętrznych</span><span class="sxs-lookup"><span data-stu-id="f31a2-102">How to disable External Groups</span></span>

<span data-ttu-id="f31a2-103">Yammer, że obsługa wiadomości zewnętrznych stosuje reguły transportu Exchange (ETRs), zestaw proaktywne kontroli w celu zapobieżenia informacje o firmie udostępnianie.</span><span class="sxs-lookup"><span data-stu-id="f31a2-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="f31a2-104">Aby ograniczyć użytkownikom możliwość tworzenia grup zewnętrznych, należy skonfigurować reguły transportu Exchange (ETR), a następnie skonfiguruj Yammer używać reguły transportu Exchange do blokowania wiadomości zewnętrznych.</span><span class="sxs-lookup"><span data-stu-id="f31a2-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="f31a2-105">Po utworzeniu reguły w Centrum administracyjnego programu Exchange w trybie Online, wykonaj następujące kroki, aby ustawić ETR do zastosowania w Yammer:</span><span class="sxs-lookup"><span data-stu-id="f31a2-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="f31a2-106">Zaloguj się na Yammer, jako zweryfikowane i w **Centrum administracyjnego Yammer**, przejdź do C **syłanych i zabezpieczenia \> ustawienia zabezpieczeń.**</span><span class="sxs-lookup"><span data-stu-id="f31a2-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="f31a2-107">W obszarze **Obsługa wiadomości zewnętrznych**, zaznacz **egzekwować swoje Exchange Online reguł transportu programu Exchange (ETRs) w Yammer.**</span><span class="sxs-lookup"><span data-stu-id="f31a2-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="f31a2-108">Wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="f31a2-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="f31a2-109">Aby uzyskać więcej informacji zobacz [Kontrola zewnętrznych, obsługa wiadomości w sieci Yammer z reguły transportu Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="f31a2-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

