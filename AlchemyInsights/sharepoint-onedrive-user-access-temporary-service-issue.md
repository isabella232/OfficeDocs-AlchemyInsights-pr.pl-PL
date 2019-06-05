---
title: Wydajność problemów programu SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719526"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="f73b3-102">SharePoint lub OneDrive wolno, niedostępne lub niedostępny dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="f73b3-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="f73b3-103">Jeśli witryny programu SharePoint lub OneDrive nie jest dostępny dla wielu użytkowników, którzy uprzednio uzyskiwała dostęp, może to być problem tymczasowy usługi.</span><span class="sxs-lookup"><span data-stu-id="f73b3-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="f73b3-104">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f73b3-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="f73b3-105">Dodaj i licencję użytkownika</span><span class="sxs-lookup"><span data-stu-id="f73b3-105">Add and license the user</span></span>

<span data-ttu-id="f73b3-106">Zapewnić, że można [przypisywać licencje dla użytkowników w usłudze Office 365 dla firm](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="f73b3-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="f73b3-107">Przypisywanie uprawnień</span><span class="sxs-lookup"><span data-stu-id="f73b3-107">Assign Permissions</span></span>

<span data-ttu-id="f73b3-108">Jeśli użytkownik został przypisany licencji programu Sharepoint i nadal otrzymuje komunikat o odmowie dostępu, upewnij się, że mają [odpowiedni poziom uprawnień](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) przypisanych.</span><span class="sxs-lookup"><span data-stu-id="f73b3-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="f73b3-109">Należy rozważyć użycie funkcji żądania dostępu</span><span class="sxs-lookup"><span data-stu-id="f73b3-109">Consider using the access request feature</span></span>

<span data-ttu-id="f73b3-110">[Funkcja żądania dostępu](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia osobom na żądanie dostępu do treści, które aktualnie nie mają uprawnień do przeglądania.</span><span class="sxs-lookup"><span data-stu-id="f73b3-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="f73b3-111">Zezwalanie na skrypt niestandardowy może powodować problemów odmowa dostępu</span><span class="sxs-lookup"><span data-stu-id="f73b3-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="f73b3-112">Istnieją pewne scenariusze, gdzie może prezentować funkcja *Zezwalaj na skrypty niestandardowe* o odmowie dostępu.</span><span class="sxs-lookup"><span data-stu-id="f73b3-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="f73b3-113">Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwości, aby wyłączyć tę funkcję.</span><span class="sxs-lookup"><span data-stu-id="f73b3-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="f73b3-114">Przejdź do strony [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="f73b3-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

