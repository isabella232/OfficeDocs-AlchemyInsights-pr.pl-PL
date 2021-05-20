---
title: Brak odnalezionych subskrypcji w Centrum zabezpieczeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544118"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="f04dd-102">Brak odnalezionych subskrypcji w Centrum zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="f04dd-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="f04dd-103">Jeśli podczas uzyskiwania dostępu Centrum zabezpieczeń usługi Microsoft Defender zostanie wyświetlony komunikat "Nie odnaleziono subskrypcji", oznacza to, że Azure Active Directory (AAD) używany do logowania użytkownika do portalu nie ma licencji usługi Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="f04dd-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="f04dd-104">Licencje Windows E5 i Office E5 to osobne licencje.</span><span class="sxs-lookup"><span data-stu-id="f04dd-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="f04dd-105">Otwórz sprawę pomocy technicznej, jeśli licencja została zakupiona, ale nie jest zapewniana obsługa techniczna dla tego wystąpienia AAD.</span><span class="sxs-lookup"><span data-stu-id="f04dd-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="f04dd-106">Masz:</span><span class="sxs-lookup"><span data-stu-id="f04dd-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="f04dd-107">Możliwy problem z inicjowaniem obsługi licencji.</span><span class="sxs-lookup"><span data-stu-id="f04dd-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="f04dd-108">Przypadkowo aprowizowano licencję do innej usługi Microsoft AAD niż ta używana do uwierzytelniania w usłudze.</span><span class="sxs-lookup"><span data-stu-id="f04dd-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>