---
title: Udzielanie użytkownikom dostępu do programu SharePoint i usługi OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677217"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="12b7a-102">Udzielanie użytkownikom dostępu do programu SharePoint i usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="12b7a-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="12b7a-103">Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to oznaczać, że wystąpił tymczasowy problem z usługą.</span><span class="sxs-lookup"><span data-stu-id="12b7a-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="12b7a-104">Sprawdź pulpit nawigacyjny kondycji usługi</span><span class="sxs-lookup"><span data-stu-id="12b7a-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="12b7a-105">Jeśli chcesz, aby osoby w Twojej organizacji mogły się logować i korzystać z programu SharePoint i usługi OneDrive, musisz dodać konta do nich i upewnić się, że mają one licencję umożliwiającą dostęp do programu SharePoint i usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="12b7a-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="12b7a-106">Najprostszym sposobem dodawania użytkowników jest centrum administracyjne Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="12b7a-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="12b7a-107">Przejdź do [strony aktywni użytkownicy w centrum administracyjnym usługi Microsoft 365](https://portal.office.com/adminportal/home#/users), a następnie kliknij pozycję **Dodaj użytkownika**.</span><span class="sxs-lookup"><span data-stu-id="12b7a-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="12b7a-108">Wprowadź informacje dotyczące użytkownika i upewnij się, że w obszarze licencje na **produkty**jest przypisana Licencja i jest zaznaczona pozycja **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="12b7a-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="12b7a-109">Pamiętaj, że Jeśli zezwolisz na udostępnianie zewnętrzne w organizacji, użytkownicy będą mogli udostępniać zawartość programu SharePoint i usługi OneDrive osobom spoza organizacji.</span><span class="sxs-lookup"><span data-stu-id="12b7a-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="12b7a-110">Nie musisz podawać tych licencji użytkownikom zewnętrznym.</span><span class="sxs-lookup"><span data-stu-id="12b7a-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="12b7a-111">Nie trzeba też dodawać do nich kont, chyba że udostępnianie jest ustawione na wartość "tylko istniejący użytkownicy zewnętrzni".</span><span class="sxs-lookup"><span data-stu-id="12b7a-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="12b7a-112">W takim przypadku, jeśli osoby nie znajdują się w katalogu organizacji, musisz dodać ich jako Gości w centrum administracyjnym usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="12b7a-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

