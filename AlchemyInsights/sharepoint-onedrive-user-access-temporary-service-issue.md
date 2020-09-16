---
title: Problemy z wydajnością — program SharePoint lub usługa OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771254"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8e87c-102">Program SharePoint lub usługa OneDrive jest wolny, niedostępny lub niedostępny dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="8e87c-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="8e87c-103">Jeśli witryna OneDrive lub SharePoint nie jest dostępna dla wielu użytkowników, którzy wcześniej mieli dostęp, może to oznaczać, że wystąpił tymczasowy problem z usługą.</span><span class="sxs-lookup"><span data-stu-id="8e87c-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8e87c-104">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8e87c-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8e87c-105">**Dodawanie i Licencjonowanie użytkownika**</span><span class="sxs-lookup"><span data-stu-id="8e87c-105">**Add and license the user**</span></span>

<span data-ttu-id="8e87c-106">Upewnij się, że [przypisujesz licencje użytkownikom w systemie Microsoft 365 dla firm](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8e87c-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="8e87c-107">**Przypisywanie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="8e87c-107">**Assign Permissions**</span></span>

<span data-ttu-id="8e87c-108">Jeśli użytkownikowi przypisano licencję programu SharePoint i nadal otrzymujesz komunikat o odmowie dostępu, upewnij się, że ma przypisany [odpowiedni poziom uprawnień](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="8e87c-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="8e87c-109">**Korzystanie z funkcji żądania dostępu**</span><span class="sxs-lookup"><span data-stu-id="8e87c-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="8e87c-110">[Funkcja żądania dostępu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umożliwia użytkownikom żądanie dostępu do zawartości, do której nie mają obecnie uprawnień.</span><span class="sxs-lookup"><span data-stu-id="8e87c-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="8e87c-111">**Zezwalaj na skrypt niestandardowy może powodować problemy z odmową dostępu**</span><span class="sxs-lookup"><span data-stu-id="8e87c-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="8e87c-112">Istnieją pewne scenariusze, w których funkcja *Zezwalaj na skrypt niestandardowy* może stanowić odmowę dostępu.</span><span class="sxs-lookup"><span data-stu-id="8e87c-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="8e87c-113">Aby uzyskać listę funkcji, których dotyczy problem, zagadnienia dotyczące zabezpieczeń i możliwość wyłączenia funkcji.</span><span class="sxs-lookup"><span data-stu-id="8e87c-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8e87c-114">Zobacz [Zezwalanie lub zapobieganie skryptowi niestandardowemu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8e87c-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

