---
title: Problem z grupami zabezpieczeń
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177627"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="0dfb9-102">Problem z grupami zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="0dfb9-102">Issue with security groups</span></span>

<span data-ttu-id="0dfb9-103">**Jeśli jest wyświetlany błąd sieci AADDS104**</span><span class="sxs-lookup"><span data-stu-id="0dfb9-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="0dfb9-104">Nieprawidłowe reguły grupy zabezpieczeń sieci są najczęstszą przyczyną błędów sieciowych w usłudze Azure Usługi domenowe w usłudze Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0dfb9-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="0dfb9-105">Grupa zabezpieczeń sieci dla sieci wirtualnej musi zezwalać na dostęp do określonych portów i protokołów.</span><span class="sxs-lookup"><span data-stu-id="0dfb9-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="0dfb9-106">Jeśli te porty są zablokowane, platforma Azure nie może monitorować ani aktualizować domeny zarządzanej.</span><span class="sxs-lookup"><span data-stu-id="0dfb9-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="0dfb9-107">Ma to również wpływ na synchronizację między usługami Azure AD AD DS Azure.</span><span class="sxs-lookup"><span data-stu-id="0dfb9-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="0dfb9-108">Upewnij się, że porty domyślne są otwarte, aby uniknąć przerw w działaniu usługi.</span><span class="sxs-lookup"><span data-stu-id="0dfb9-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="0dfb9-109">Aby zrozumieć i rozwiązać typowe alerty dotyczące problemów z konfiguracją grupy zabezpieczeń sieci, zobacz [Dodawanie i weryfikowanie grup zabezpieczeń.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="0dfb9-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
