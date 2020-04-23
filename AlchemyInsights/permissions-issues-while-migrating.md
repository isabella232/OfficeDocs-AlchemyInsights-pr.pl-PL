---
title: Problemy z uprawnieniami podczas migracji
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 077b7cf29ef6a40ef7f2aebef15e39a0f5df0fc3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758980"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="24952-102">Synchronizacja profilu użytkownika i zdjęć</span><span class="sxs-lookup"><span data-stu-id="24952-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="24952-103">**Synchronizacja zdjęć profilowych** — użytkownicy mogą zauważyć, że ich zdjęcie profilowe nie jest synchronizowane z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="24952-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="24952-104">Być może próbowali zaktualizować swoje zdjęcie profilowe, a zdjęcie nadal pojawia się jako stare zdjęcie.</span><span class="sxs-lookup"><span data-stu-id="24952-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="24952-105">Aby upewnić się, że zdjęcie profilowe będzie wyświetlane zgodnie z oczekiwaniami, użytkownik będzie musiał zainicjować synchronizację zdjęć.</span><span class="sxs-lookup"><span data-stu-id="24952-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="24952-106">Aby uzyskać więcej informacji na temat procesu synchronizacji zdjęć, zobacz [Informacje o synchronizacji zdjęć profilowych w usłudze Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="24952-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="24952-107">**Synchronizacja profilu** — czas wymagany do ukończenia synchronizacji profilu zależy od liczby zmian (pracy), które ma przetworzyć zadanie importu usługi AD.</span><span class="sxs-lookup"><span data-stu-id="24952-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="24952-108">Jeśli istnieje wiele zmian, zadanie czasomierza ma dużo pracy do zrobienia, a to zajmie więcej czasu, aby zmiany zostały odzwierciedlone w aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="24952-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="24952-109">Jeśli zadanie czasomierza ma niewielką ilość pracy do wykonania, zmiany zostaną odzwierciedlone w aplikacji profilu użytkownika znacznie szybciej.</span><span class="sxs-lookup"><span data-stu-id="24952-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="24952-110">Aby uzyskać więcej informacji na temat procesu synchronizacji profilu, zobacz [Informacje o synchronizacji profilu użytkownika w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="24952-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="24952-111">**Aktualizuj profil w aplikacji Office Delve** — użytkownicy aplikacji Delve mogą zarządzać profilem usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="24952-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="24952-112">Aby uzyskać więcej informacji, zobacz [Wyświetlanie i aktualizowanie profilu w aplikacji Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="24952-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

