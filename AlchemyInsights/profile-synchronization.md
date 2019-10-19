---
title: Synchronizacja profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554343"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="f65d9-102">Kiedy mój profil zmienia synchronizację z aplikacją profilu użytkownika programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="f65d9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="f65d9-103">Program SharePoint Online używa zadania czasomierza importu usługi Active Directory (AD import) do importowania użytkowników i grup do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f65d9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="f65d9-104">Import AD synchronizuje zmiany z magazynu usługi SharePoint Online Directory do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f65d9-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="f65d9-105">Te zmiany są przetwarzane w partiach.</span><span class="sxs-lookup"><span data-stu-id="f65d9-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="f65d9-106">Zadanie czasomierza jest uruchamiane, dopóki zmiany są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="f65d9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="f65d9-107">Czas potrzebny do uruchomienia zadania zależy od liczby zmian do przetworzenia.</span><span class="sxs-lookup"><span data-stu-id="f65d9-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="f65d9-108">Duża liczba zmian trwa dłużej.</span><span class="sxs-lookup"><span data-stu-id="f65d9-108">A large number of changes takes longer.</span></span> <span data-ttu-id="f65d9-109">Umowa dotycząca poziomu usług (SLA) stwierdza, że zmiana użytkownika w katalogu online programu SharePoint zostaną uwzględnione w aplikacji profilu użytkownika w ciągu 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="f65d9-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="f65d9-110">Więcej informacji o synchronizacji profilu użytkownika w programie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f65d9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

