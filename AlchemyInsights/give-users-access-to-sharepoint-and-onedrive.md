---
title: Zapewnienie użytkownikom dostępu do programu SharePoint i usługi OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36523773"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="ec419-102">Zapewnienie użytkownikom dostępu do programu SharePoint i usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="ec419-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="ec419-103">Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być problem tymczasowy usługi.</span><span class="sxs-lookup"><span data-stu-id="ec419-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="ec419-104">Sprawdź pulpit nawigacyjny kondycji usługi</span><span class="sxs-lookup"><span data-stu-id="ec419-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="ec419-105">Jeśli chcesz, aby osoby w organizacji mogły logować się i używać programu SharePoint i usługi OneDrive, musisz dodać do nich konta i upewnić się, że mają licencję, która daje im dostęp do programu SharePoint i usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ec419-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="ec419-106">Najprostszym sposobem dodawania użytkowników znajduje się w centrum administracyjnym Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ec419-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="ec419-107">Przejdź do [strony aktywnych użytkowników w centrum administracyjnym Microsoft 365](https://portal.office.com/adminportal/home#/users), a następnie kliknij przycisk **Dodaj użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="ec419-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="ec419-108">Wypełnij informacje dla użytkownika i upewnij się, że w obszarze **licencje produktu**, licencja jest przypisany i **SharePoint Online** jest zaznaczone.</span><span class="sxs-lookup"><span data-stu-id="ec419-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="ec419-109">Należy pamiętać, że Jeśli zezwolisz na udostępnianie zewnętrzne w organizacji, użytkownicy mogą udostępniać zawartość programu SharePoint i usługi OneDrive osobom spoza organizacji.</span><span class="sxs-lookup"><span data-stu-id="ec419-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="ec419-110">Nie musisz udzielać tych licencji użytkownikom zewnętrznym.</span><span class="sxs-lookup"><span data-stu-id="ec419-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="ec419-111">Nie trzeba też dodawać kont dla nich, chyba że udostępnianie jest ustawione na "tylko istniejący użytkownicy zewnętrzni".</span><span class="sxs-lookup"><span data-stu-id="ec419-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="ec419-112">W takim przypadku jeśli ludzie nie są w katalogu organizacji, należy dodać je jako gość w centrum administracyjnym usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ec419-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

