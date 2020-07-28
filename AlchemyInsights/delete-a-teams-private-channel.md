---
title: Usuwanie kanału prywatnego teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439919"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="4b965-102">Usuwanie kanału prywatnego teams</span><span class="sxs-lookup"><span data-stu-id="4b965-102">Delete a Teams private channel</span></span>

<span data-ttu-id="4b965-103">Firma Microsoft jest świadoma problemu z usunięciem kanału prywatnego usługi Teams, jeśli w podstawowej witrynie programu SharePoint włączono zasady przechowywania programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b965-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="4b965-104">Firma Microsoft pracuje nad poprawką.</span><span class="sxs-lookup"><span data-stu-id="4b965-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="4b965-105">W międzyczasie można użyć następujących obejść, aby usunąć kanał prywatny.</span><span class="sxs-lookup"><span data-stu-id="4b965-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="4b965-106">**Wyklucz zespół/zbiór witryn z zasad przechowywania programu Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="4b965-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="4b965-107">Przejdź do portalu administracyjnego usługi Office 365 i wybierz pozycję **Pokaż wszystko** w lewym okienku nawigacji.</span><span class="sxs-lookup"><span data-stu-id="4b965-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="4b965-108">W **obszarze Centra administracyjne**przejdź do pozycji Zasady zapobiegania utracie danych **dotyczących zgodności &**  >  **Data Loss Prevention**  >  **Policy**bezpieczeństwa .</span><span class="sxs-lookup"><span data-stu-id="4b965-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="4b965-109">Zidentyfikuj wszystkie zasady, które mają zastosowanie do witryn programu Sharepoint, i zmodyfikuj zasady, aby witryna programu SharePoint dla zespołu zawierającego kanał prywatny NIE została uwzględniona w zasadach przechowywania.</span><span class="sxs-lookup"><span data-stu-id="4b965-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="4b965-110">Zapisz zasady.</span><span class="sxs-lookup"><span data-stu-id="4b965-110">Save the policy.</span></span>
    <span data-ttu-id="4b965-111">Wprowadzanie ustawień zasad może potrwać do 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="4b965-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="4b965-112">Po wykluczeniu witryny można usunąć kanał prywatny.</span><span class="sxs-lookup"><span data-stu-id="4b965-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="4b965-113">Możesz ***might*** usunąć kanał prywatny przy użyciu usługi Microsoft Teams na urządzeniu z systemem Android.</span><span class="sxs-lookup"><span data-stu-id="4b965-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="4b965-114">Aby uzyskać powiązane informacje o programie SharePoint, zobacz [Nie można usunąć elementów w usłudze SharePoint Online lub usłudze OneDrive dla Firm](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="4b965-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>