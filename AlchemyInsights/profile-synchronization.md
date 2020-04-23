---
title: Synchronizacja profilu
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768123"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="dd5ad-102">Kiedy zmiany profilu są synchronizowane z aplikacją profilu użytkownika programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="dd5ad-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="dd5ad-103">Usługa SharePoint Online używa zadania czasomierza importu usługi Active Directory (Import usługi AD) do importowania użytkowników i grup do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="dd5ad-104">Import usługi AD synchronizuje zmiany ze sklepu sharepoint online do aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="dd5ad-105">Zmiany te są przetwarzane w partiach.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="dd5ad-106">Zadanie czasomierza jest uruchamiane do momentu zsynchronizowania zmian.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="dd5ad-107">Czas potrzebny do uruchomienia zadania zależy od liczby zmian do przetworzenia.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="dd5ad-108">Duża liczba zmian trwa dłużej.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-108">A large number of changes takes longer.</span></span> <span data-ttu-id="dd5ad-109">Umowa dotyczącej poziomu usług (SLA) stanowi, że zmiana użytkownika w katalogu SharePoint Online zostanie odzwierciedlona w aplikacji profilu użytkownika w ciągu 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="dd5ad-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="dd5ad-110">Więcej informacji o synchronizacji profilu użytkownika w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dd5ad-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

