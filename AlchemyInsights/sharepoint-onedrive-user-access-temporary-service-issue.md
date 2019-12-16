---
title: Problemy z wydajnością-SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053811"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c96d0-102">SharePoint lub OneDrive powolne, niedostępne lub niedostępne dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="c96d0-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="c96d0-103">Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być problem tymczasowy usługi.</span><span class="sxs-lookup"><span data-stu-id="c96d0-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="c96d0-104">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c96d0-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="c96d0-105">**Dodawanie i Licencjonowanie użytkownika**</span><span class="sxs-lookup"><span data-stu-id="c96d0-105">**Add and license the user**</span></span>

<span data-ttu-id="c96d0-106">Upewnij się, że [Przypisywanie licencji użytkownikom w pakiecie Office 365 dla firm](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c96d0-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="c96d0-107">**Przypisywanie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="c96d0-107">**Assign Permissions**</span></span>

<span data-ttu-id="c96d0-108">Jeśli użytkownik ma przypisaną licencję programu SharePoint i nadal odbiera komunikat o odmowie dostępu, upewnij się, że ma przypisany [odpowiedni poziom uprawnień](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="c96d0-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="c96d0-109">**Rozważ użycie funkcji żądania dostępu**</span><span class="sxs-lookup"><span data-stu-id="c96d0-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="c96d0-110">[Funkcja żądania dostępu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia użytkownikom żądanie dostępu do zawartości, której obecnie nie ma uprawnień do zobaczenia.</span><span class="sxs-lookup"><span data-stu-id="c96d0-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="c96d0-111">**Zezwalaj na niestandardowy skrypt może spowodować problemy z odmową dostępu**</span><span class="sxs-lookup"><span data-stu-id="c96d0-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="c96d0-112">Istnieją pewne scenariusze, w których funkcja *Zezwalaj na skrypt niestandardowy* może przedstawiać odmowa dostępu.</span><span class="sxs-lookup"><span data-stu-id="c96d0-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="c96d0-113">Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwość wyłączenia tej funkcji.</span><span class="sxs-lookup"><span data-stu-id="c96d0-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="c96d0-114">Odwiedź stronę [Zezwalaj lub Zapobiegaj skryptowaniu niestandardowym](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="c96d0-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

