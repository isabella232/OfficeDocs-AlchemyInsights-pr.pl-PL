---
title: Synchronizacji profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554343"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="89f91-102">Kiedy moje zmiany profilu synchronizację aplikacji profilu użytkownika programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="89f91-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="89f91-103">SharePoint Online używa zadanie czasomierza importu usługi Active Directory (AD Import) do importowania użytkowników i grup do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="89f91-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="89f91-104">Importuj AD synchronizuje zmiany z magazynu katalogu Online programu SharePoint do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="89f91-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="89f91-105">Te zmiany są przetwarzane w plikach wsadowych.</span><span class="sxs-lookup"><span data-stu-id="89f91-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="89f91-106">Zadanie czasomierza jest uruchamiany, dopóki zmiany są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="89f91-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="89f91-107">Czas uruchomienia zadania zależy od liczby zmian do procesu.</span><span class="sxs-lookup"><span data-stu-id="89f91-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="89f91-108">Dużej liczby zmian trwa dłużej.</span><span class="sxs-lookup"><span data-stu-id="89f91-108">A large number of changes takes longer.</span></span> <span data-ttu-id="89f91-109">Umowy poziomu usług (SLA) stwierdza, że zmiany do użytkownika w katalogu Online programu SharePoint będą uwzględniane w aplikacji profilu użytkownika w ciągu 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="89f91-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="89f91-110">Więcej informacji o synchronizacji profilu użytkownika w dokumentacji Online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="89f91-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

