---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418479"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="0c230-102">Monitorowanie dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="0c230-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="0c230-103">Użytkownicy kierowana do dostępu warunkowego otrzymają wiadomość e-mail z powiadomieniem, jeżeli nie spełniają one wymagań dostępu organizacji.</span><span class="sxs-lookup"><span data-stu-id="0c230-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0c230-104">Aby rozwiązać, zaleca się jeden lub kilka z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="0c230-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0c230-105">W przypadku przyjmuje się, że urządzenie się zarejestrować, należy poinformować użytkownika, aby przejść do aplikacji Portal firmy i sprawdź, czy pojawia się w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="0c230-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0c230-106">Jeśli tak nie jest, użytkownik należy zarejestrować urządzenia.</span><span class="sxs-lookup"><span data-stu-id="0c230-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0c230-107">W portalu Azure przejdź do **Intune \> zgodności urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="0c230-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0c230-108">W obszarze **monitora** kliknij **zgodności urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="0c230-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="0c230-109">Wyświetlanie raportu zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczony jako zgodny z.</span><span class="sxs-lookup"><span data-stu-id="0c230-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0c230-110">W portalu Azure przejdź do **Intune \> zgodności urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="0c230-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0c230-111">W obszarze **Zarządzaj**kliknij **zasady**.</span><span class="sxs-lookup"><span data-stu-id="0c230-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="0c230-112">Na liście zasady zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="0c230-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0c230-113">Jeżeli żaden profil nie jest przypisany, Intune nie będzie mógł potwierdzić stan zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="0c230-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0c230-114">Edytuj przypisanie warunkowego dostępu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="0c230-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0c230-115">W portalu Azure przejdź do **Intune \> dostępu warunkowego \> zasady**</span><span class="sxs-lookup"><span data-stu-id="0c230-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0c230-116">Wybierz zasadę z listy</span><span class="sxs-lookup"><span data-stu-id="0c230-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0c230-117">Kliknij przycisk **Użytkownicy i grupy**</span><span class="sxs-lookup"><span data-stu-id="0c230-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0c230-118">Aby skierować pewną politykę na kogoś, należy dodać je do listy **dołączania** .</span><span class="sxs-lookup"><span data-stu-id="0c230-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="0c230-119">W celu zapewnienia, że osoba zostanie pominięty, z zasady, należy dodać je do listy **wykluczeń** .</span><span class="sxs-lookup"><span data-stu-id="0c230-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0c230-120">Przeczytaj więcej: [jak urządzeń dostępu warunkowego monitora](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0c230-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

