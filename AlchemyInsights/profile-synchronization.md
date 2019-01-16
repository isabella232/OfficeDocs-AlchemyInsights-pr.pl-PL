---
title: Synchronizacji profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304407"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="890df-102">Kiedy moje zmiany profilu synchronizację aplikacji profilu użytkownika programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="890df-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="890df-103">SharePoint Online używa zadanie czasomierza importu usługi Active Directory (AD Import) do importowania użytkowników i grup do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="890df-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="890df-p101">Importuj AD synchronizuje zmiany z magazynu katalogu Online programu SharePoint do aplikacji profilu użytkownika. Te zmiany są przetwarzane w plikach wsadowych.</span><span class="sxs-lookup"><span data-stu-id="890df-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="890df-106">Zadanie czasomierza jest uruchamiany, dopóki zmiany są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="890df-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="890df-p102">Czas uruchomienia zadania zależy od liczby zmian do procesu. Dużej liczby zmian trwa dłużej. Umowy poziomu usług (SLA) stwierdza, że zmiany do użytkownika w katalogu Online programu SharePoint będą uwzględniane w aplikacji profilu użytkownika w ciągu 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="890df-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="890df-110">Więcej informacji o synchronizacji profilu użytkownika w dokumentacji Online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="890df-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

