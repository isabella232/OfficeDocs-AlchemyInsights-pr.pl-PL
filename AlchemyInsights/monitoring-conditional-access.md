---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713728"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="47480-102">Monitorowanie dostępu warunkowego dla programu Exchange</span><span class="sxs-lookup"><span data-stu-id="47480-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="47480-103">Użytkownicy objęci dostępem warunkowym otrzymają wiadomość e-mail z powiadomieniem, jeśli nie spełniają wymagań dotyczących dostępu w organizacji.</span><span class="sxs-lookup"><span data-stu-id="47480-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="47480-104">Aby rozwiązać problem, zaleca się co najmniej jedno z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="47480-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="47480-105">Jeśli zakłada się, że urządzenie jest zarejestrowane, poinformuj go o tym, aby przejść do aplikacji Portal firmy i sprawdzić, czy jest ono wyświetlane w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="47480-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="47480-106">Jeśli tak nie jest, użytkownik powinien zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="47480-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="47480-107">W witrynie Azure portal przejdź do \*\*zgodności urządzenia usługi Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="47480-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="47480-108">W obszarze **Monitor kliknij** pozycję **Zgodność urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="47480-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="47480-109">Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne.</span><span class="sxs-lookup"><span data-stu-id="47480-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="47480-110">W witrynie Azure portal przejdź do \*\*zgodności urządzenia usługi Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="47480-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="47480-111">W obszarze **Zarządzanie**kliknij pozycję **Zasady**.</span><span class="sxs-lookup"><span data-stu-id="47480-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="47480-112">Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="47480-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="47480-113">Jeśli nie zostanie przypisany żaden profil, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="47480-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="47480-114">Edytuj przypisanie dostępu warunkowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="47480-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="47480-115">W witrynie Azure Portal przejdź do **zasad dostępu \> \> warunkowego usługi Intune**</span><span class="sxs-lookup"><span data-stu-id="47480-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="47480-116">Wybieranie zasad z listy</span><span class="sxs-lookup"><span data-stu-id="47480-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="47480-117">Kliknij **pozycję Użytkownicy i grupy**</span><span class="sxs-lookup"><span data-stu-id="47480-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="47480-118">Aby skierować do innej osoby określone zasady, dodaj je do listy **Dołącz.**</span><span class="sxs-lookup"><span data-stu-id="47480-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="47480-119">Aby upewnić się, że dana osoba została pominięta w zasadach, dodaj ją do listy **Wyklucz.**</span><span class="sxs-lookup"><span data-stu-id="47480-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="47480-120">Czytaj więcej: [Jak monitorować urządzenia dostępu warunkowego](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="47480-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

