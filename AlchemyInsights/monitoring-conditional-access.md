---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702913"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="958cb-102">Monitorowanie dostępu warunkowego dla programu Exchange</span><span class="sxs-lookup"><span data-stu-id="958cb-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="958cb-103">Użytkownicy ukierunkowany na dostęp warunkowy otrzymają powiadomienie pocztą e-mail, jeśli nie spełnią wymagań organizacji dotyczących dostępu.</span><span class="sxs-lookup"><span data-stu-id="958cb-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="958cb-104">W celu rozwiązania problemu zalecamy co najmniej jedno z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="958cb-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="958cb-105">Jeśli urządzenie jest uważane za zarejestrowane, zaleca się, aby użytkownik przeszedł do aplikacji Portal firmy i upewnić się, że jest wyświetlany w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="958cb-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="958cb-106">Jeśli nie, użytkownik powinien zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="958cb-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="958cb-107">W portalu Azure przejdź do obszaru usługi Intune dotyczącego \*\* \> zgodności\*\*.</span><span class="sxs-lookup"><span data-stu-id="958cb-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="958cb-108">W obszarze **monitor** kliknij pozycję **zgodność urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="958cb-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="958cb-109">Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne.</span><span class="sxs-lookup"><span data-stu-id="958cb-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="958cb-110">W portalu Azure przejdź do obszaru usługi Intune dotyczącego \*\* \> zgodności\*\*.</span><span class="sxs-lookup"><span data-stu-id="958cb-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="958cb-111">W obszarze **Zarządzanie**kliknij pozycję **zasady**.</span><span class="sxs-lookup"><span data-stu-id="958cb-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="958cb-112">Na liście zasad zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="958cb-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="958cb-113">Jeśli żaden profil nie jest przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="958cb-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="958cb-114">Edytowanie przydziału dostępu warunkowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="958cb-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="958cb-115">W portalu Azure Portal przejdź do \*\* \> \> zasad dostępu warunkowego usługi Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="958cb-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="958cb-116">Wybierz zasadę z listy</span><span class="sxs-lookup"><span data-stu-id="958cb-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="958cb-117">Kliknij pozycję **Użytkownicy i grupy**</span><span class="sxs-lookup"><span data-stu-id="958cb-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="958cb-118">Aby określić zasady jako docelowe dla określonej osoby, Dodaj je do listy **dołączania** .</span><span class="sxs-lookup"><span data-stu-id="958cb-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="958cb-119">Aby upewnić się, że dana osoba zostanie pominięta w zasadach, Dodaj je do listy **wykluczania** .</span><span class="sxs-lookup"><span data-stu-id="958cb-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="958cb-120">Dowiedz się więcej: [Jak monitorować urządzenia z dostępem warunkowym](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="958cb-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

