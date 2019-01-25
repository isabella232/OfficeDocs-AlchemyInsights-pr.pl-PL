---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482443"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="4d982-102">Monitorowanie dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="4d982-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="4d982-p101">Użytkownicy kierowana do dostępu warunkowego otrzymają wiadomość e-mail z powiadomieniem, jeżeli nie spełniają one wymagań dostępu organizacji. Aby rozwiązać, zaleca się jeden lub kilka z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="4d982-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="4d982-p102">W przypadku przyjmuje się, że urządzenie się zarejestrować, należy poinformować użytkownika, aby przejść do aplikacji Portal firmy i sprawdź, czy pojawia się w portalu firmy. Jeśli tak nie jest, użytkownik należy zarejestrować urządzenia.</span><span class="sxs-lookup"><span data-stu-id="4d982-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="4d982-p103">W portalu Azure przejdź do **Intune \> zgodności urządzenia**. W obszarze **monitora** kliknij **zgodności urządzenia**. Wyświetlanie raportu zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczony jako zgodny z.</span><span class="sxs-lookup"><span data-stu-id="4d982-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="4d982-p104">W portalu Azure przejdź do **Intune \> zgodności urządzenia**. W obszarze **Zarządzaj**kliknij **zasady**. Na liście zasady zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeżeli żaden profil nie jest przypisany, Intune nie będzie mógł potwierdzić stan zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="4d982-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="4d982-114">Edytuj przypisanie warunkowego dostępu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="4d982-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="4d982-115">W portalu Azure przejdź do **Intune \> dostępu warunkowego \> zasady**</span><span class="sxs-lookup"><span data-stu-id="4d982-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="4d982-116">Wybierz zasadę z listy</span><span class="sxs-lookup"><span data-stu-id="4d982-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="4d982-117">Kliknij przycisk **Użytkownicy i grupy**</span><span class="sxs-lookup"><span data-stu-id="4d982-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="4d982-p105">Aby skierować pewną politykę na kogoś, należy dodać je do listy **dołączania** . W celu zapewnienia, że osoba zostanie pominięty, z zasady, należy dodać je do listy **wykluczeń** .</span><span class="sxs-lookup"><span data-stu-id="4d982-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="4d982-120">Przeczytaj więcej: [jak urządzeń dostępu warunkowego monitora](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="4d982-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

