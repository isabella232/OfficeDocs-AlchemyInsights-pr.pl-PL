---
title: Problemy z uprawnieniami podczas przeprowadzania migracji
ms.author: kirks
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 3cdf5909595b5b1fac9aeb00865546c1dcff5f09
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372174"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="16653-102">Synchronizacja profilu użytkownika i zdjęcie</span><span class="sxs-lookup"><span data-stu-id="16653-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="16653-103">**Synchronizacji profilu fotografii** - użytkownicy mogą zauważyć, że swoje zdjęcie w profilu nie jest zsynchronizowany w programie SharePoint.</span><span class="sxs-lookup"><span data-stu-id="16653-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="16653-104">Lub, próbowali zaktualizować swoje zdjęcie w profilu, zdjęcie nadal pojawia się jako stare zdjęcie.</span><span class="sxs-lookup"><span data-stu-id="16653-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="16653-105">Aby zapewnić, że zdjęcie profilu pokazuje zgodnie z oczekiwaniami, użytkownik będzie musiał rozpocząć synchronizację zdjęcie.</span><span class="sxs-lookup"><span data-stu-id="16653-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="16653-106">Aby uzyskać więcej informacji na temat procesu synchronizacji fotografii zobacz [informacje o synchronizacji obraz profilu w usłudze Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="16653-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="16653-107">**Synchronizacja profilu użytkownika** - czasu wymaganego do wykonania synchronizacji profilu użytkownika zależy od liczby zmian (praca) zadania importu AD ma do procesu.</span><span class="sxs-lookup"><span data-stu-id="16653-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="16653-108">Jeśli istnieje wiele zmian, zadanie czasomierza ma wiele do zrobienia, i będzie trwało dłużej, zmiany są odzwierciedlane w aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="16653-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="16653-109">Jeśli zadanie czasomierza ma niewielką ilość pracy, zmiany zostaną odzwierciedlone w aplikacji profilu użytkownika znacznie szybciej.</span><span class="sxs-lookup"><span data-stu-id="16653-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="16653-110">Aby uzyskać więcej informacji na temat procesu synchronizacji profilu zobacz [informacje o synchronizacji profilu użytkownika w dokumentacji Online programu SharePoint](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="16653-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="16653-111">**Aktualizacja profilu w Wkrocz pakietu Office** - Wkrocz użytkownicy mogą zarządzać swoim profilu pakietu Office 365.</span><span class="sxs-lookup"><span data-stu-id="16653-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="16653-112">Aby uzyskać więcej informacji zobacz [Zobacz i Edytuj swój profil w Wkrocz pakietu Office](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="16653-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

