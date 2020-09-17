---
title: Problemy z uprawnieniami podczas migrowania
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798062"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="ab478-102">Profil użytkownika i Synchronizacja zdjęć</span><span class="sxs-lookup"><span data-stu-id="ab478-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="ab478-103">**Synchronizacja zdjęć profilu** — użytkownicy mogą zauważyć, że ich zdjęcie profilu nie jest synchronizowane z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab478-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="ab478-104">Mogą też próbować zaktualizować swoje zdjęcie profilu, a zdjęcie będzie nadal wyświetlane jako stare zdjęcie.</span><span class="sxs-lookup"><span data-stu-id="ab478-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="ab478-105">Aby upewnić się, że zdjęcie profilu jest wyświetlane zgodnie z oczekiwaniami, użytkownik będzie musiał rozpocząć synchronizację zdjęć.</span><span class="sxs-lookup"><span data-stu-id="ab478-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="ab478-106">Aby uzyskać więcej informacji na temat procesu synchronizacji zdjęć, zobacz [Informacje o synchronizacji obrazów profilu w programie Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="ab478-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="ab478-107">**Synchronizacja profilu** — czas wymagany do ukończenia synchronizacji profilu zależy od liczby zmian (pracy), które mają zostać przetworzone przez zadanie importu AD.</span><span class="sxs-lookup"><span data-stu-id="ab478-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="ab478-108">W przypadku wielu zmian zadanie czasomierza ma wiele pracy do wykonania, a zmiany zostaną odzwierciedlone w aplikacji profilu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="ab478-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="ab478-109">Jeśli zadanie czasomierza ma niewielką ilość pracy do wykonania, zmiany zostaną odzwierciedlone w aplikacji profilu użytkownika znacznie szybciej.</span><span class="sxs-lookup"><span data-stu-id="ab478-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="ab478-110">Aby uzyskać więcej informacji na temat procesu synchronizacji profilu, zobacz [informacje na temat synchronizacji profilu użytkownika w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="ab478-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="ab478-111">**Aktualizowanie profilu w aplikacji Office Delve** — użytkownicy aplikacji Delve mogą zarządzać profilem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ab478-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="ab478-112">Aby uzyskać więcej informacji, zobacz [Wyświetlanie i aktualizowanie profilu w aplikacji Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="ab478-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

