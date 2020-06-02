---
title: Problemy z wydajnością — program SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511158"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a1ec5-102">Program SharePoint lub OneDrive są powolne, niedostępne lub niedostępne dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="a1ec5-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="a1ec5-103">Jeśli witryna usługi OneDrive lub programu SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być tymczasowy problem z usługą.</span><span class="sxs-lookup"><span data-stu-id="a1ec5-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a1ec5-104">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a1ec5-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="a1ec5-105">**Dodawanie i licencjonowanie użytkownika**</span><span class="sxs-lookup"><span data-stu-id="a1ec5-105">**Add and license the user**</span></span>

<span data-ttu-id="a1ec5-106">Upewnij się, że [licencje są przypisywane użytkownikom w usłudze Microsoft 365 dla firm](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a1ec5-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="a1ec5-107">**Przypisywanie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="a1ec5-107">**Assign Permissions**</span></span>

<span data-ttu-id="a1ec5-108">Jeśli użytkownikowi przypisano licencję programu Sharepoint i nadal otrzymuje komunikat o odmowie dostępu, upewnij się, że ma przypisany [odpowiedni poziom uprawnień.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="a1ec5-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="a1ec5-109">**Rozważ użycie funkcji żądania dostępu**</span><span class="sxs-lookup"><span data-stu-id="a1ec5-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="a1ec5-110">[Funkcja żądania dostępu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia użytkownikom żądanie dostępu do zawartości, do których obecnie nie mają uprawnień.</span><span class="sxs-lookup"><span data-stu-id="a1ec5-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="a1ec5-111">**Zezwalaj na skrypt niestandardowy może powodować problemy z odmową dostępu**</span><span class="sxs-lookup"><span data-stu-id="a1ec5-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="a1ec5-112">Istnieją pewne scenariusze, w których *funkcja Zezwalaj na skrypt niestandardowy* może przedstawiać odmowę dostępu.</span><span class="sxs-lookup"><span data-stu-id="a1ec5-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="a1ec5-113">Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwość wyłączenia tej funkcji.</span><span class="sxs-lookup"><span data-stu-id="a1ec5-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a1ec5-114">Odwiedź stronę [Zezwalaj lub zapobiegaj skrypcowaniu niestandardowemu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="a1ec5-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

