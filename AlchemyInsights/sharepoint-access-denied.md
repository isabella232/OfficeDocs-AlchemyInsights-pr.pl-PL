---
title: Rozwiązywanie problemów z wiadomościami odmowa dostępu
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735747"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="a79f8-102">Rozwiązywanie problemów z wiadomościami odmowa dostępu</span><span class="sxs-lookup"><span data-stu-id="a79f8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="a79f8-103">Jeśli otrzymujesz podczas próby przeglądania witryny programu Sharepoint w trybie Online komunikat o odmowie dostępu, zapoznaj się z punktem poniżej artykułów.</span><span class="sxs-lookup"><span data-stu-id="a79f8-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="a79f8-104">Dodaj i licencję użytkownika</span><span class="sxs-lookup"><span data-stu-id="a79f8-104">Add and License the user</span></span>

<span data-ttu-id="a79f8-105">Zapewnić, że można [przypisywać licencje dla użytkowników w usłudze Office 365 dla firm](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="a79f8-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="a79f8-106">Przypisywanie uprawnień</span><span class="sxs-lookup"><span data-stu-id="a79f8-106">Assign Permissions</span></span>

<span data-ttu-id="a79f8-107">Jeśli użytkownik został przypisany licencji programu Sharepoint i nadal otrzymuje komunikat o odmowie dostępu, upewnij się, że mają [przypisany odpowiedni poziom uprawnień](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a79f8-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="a79f8-108">Należy rozważyć użycie funkcji żądania dostępu</span><span class="sxs-lookup"><span data-stu-id="a79f8-108">Consider using the access request feature</span></span>

<span data-ttu-id="a79f8-109">Funkcji [żądania dostępu](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia osobom na żądanie dostępu do treści, które aktualnie nie mają uprawnień do przeglądania.</span><span class="sxs-lookup"><span data-stu-id="a79f8-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="a79f8-110">Zezwalanie na skrypt niestandardowy może powodować problemów odmowa dostępu</span><span class="sxs-lookup"><span data-stu-id="a79f8-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="a79f8-111">Istnieją pewne scenariusze, gdzie może prezentować funkcji "Zezwalaj na skrypt niestandardowy" o odmowie dostępu.</span><span class="sxs-lookup"><span data-stu-id="a79f8-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="a79f8-112">Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwości, aby wyłączyć tę funkcję.</span><span class="sxs-lookup"><span data-stu-id="a79f8-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a79f8-113">Odwiedź witrynę, [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="a79f8-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="a79f8-114">Uwaga: Jeśli witryny programu SharePoint lub OneDrive nie jest dostępny dla wielu użytkowników, którzy uprzednio uzyskiwała dostęp, może istnieć problem tymczasowej usługi.</span><span class="sxs-lookup"><span data-stu-id="a79f8-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a79f8-115">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a79f8-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

