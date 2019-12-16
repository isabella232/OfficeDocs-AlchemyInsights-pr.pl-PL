---
title: Problemy z uprawnieniami podczas migracji
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054424"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="6b290-102">Synchronizacja profilu użytkownika i zdjęcia</span><span class="sxs-lookup"><span data-stu-id="6b290-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="6b290-103">**Synchronizacja zdjęć profilowych** -użytkownicy mogą zauważyć, że ich zdjęcie profilowe nie synchronizuje się z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6b290-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="6b290-104">Lub mogą próbowali zaktualizować swoje zdjęcie profilowe, a zdjęcie nadal pojawia się jako stare zdjęcie.</span><span class="sxs-lookup"><span data-stu-id="6b290-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="6b290-105">Aby upewnić się, że zdjęcie profilowe jest wyświetlane zgodnie z oczekiwaniami, użytkownik będzie musiał zainicjować synchronizację zdjęć.</span><span class="sxs-lookup"><span data-stu-id="6b290-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="6b290-106">Aby uzyskać więcej informacji o procesie synchronizacji zdjęć, zobacz [Informacje o synchronizacji obrazu profilu w pakiecie Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="6b290-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="6b290-107">**Synchronizacja profilu** — czas wymagany do ukończenia synchronizacji profilu zależy od liczby zmian (pracy) zadania importu AD musi przetworzyć.</span><span class="sxs-lookup"><span data-stu-id="6b290-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="6b290-108">Jeśli istnieje wiele zmian, zadanie czasomierza ma dużo pracy do zrobienia i zajmie więcej zmian, które mają być odzwierciedlone w aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6b290-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="6b290-109">Jeśli zadanie czasomierza ma małą ilość pracy do zrobienia, zmiany zostaną odzwierciedlone w aplikacji profilu użytkownika znacznie szybciej.</span><span class="sxs-lookup"><span data-stu-id="6b290-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="6b290-110">Aby uzyskać więcej informacji na temat procesu synchronizacji profilu zobacz [Informacje o synchronizacji profilu użytkownika w programie SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="6b290-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="6b290-111">**Aktualizowanie profilu w pakiecie Office Delve** — użytkownicy programu Delve mogą zarządzać swoim profilem 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="6b290-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="6b290-112">Aby uzyskać więcej informacji, zobacz temat [Wyświetlanie i aktualizowanie profilu w pakiecie Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="6b290-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

