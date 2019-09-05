---
title: Rozwiązywanie problemów z komunikatami odmowa dostępu
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751286"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="eb812-102">Rozwiązywanie problemów z odmową dostępu wiadomości w centrum administracyjnym programu SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="eb812-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="eb812-103">Jeśli otrzymujesz komunikat o odmowie dostępu podczas próby przejdź do centrum administracyjnego programu SharePoint/OneDrive, upewnij się, że [przypisać licencję do użytkownika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="eb812-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="eb812-104">Jeśli użytkownik ma licencję, należy również upewnić się, że [przypisano rolę administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , która może uzyskiwać dostęp do centrów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="eb812-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="eb812-105">Ten problem może również wystąpić, gdy użytkownik zostanie usunięty i utworzony ponownie z tej samej głównej nazwy użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="eb812-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="eb812-106">Nowe konto jest tworzone przy użyciu innego PUID (Passport Unique ID) wartość.</span><span class="sxs-lookup"><span data-stu-id="eb812-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="eb812-107">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID.</span><span class="sxs-lookup"><span data-stu-id="eb812-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="eb812-108">Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną (OU) usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eb812-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="eb812-109">Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie są przenoszone do innej jednostki organizacyjnej i resynced z programu SharePoint, mogą wystąpić ten problem.</span><span class="sxs-lookup"><span data-stu-id="eb812-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="eb812-110">Aby rozwiązać ten problem, należy przywrócić oryginalną nazwę UPN z krokami w artykule, [Przywróć użytkownika w pakiecie Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="eb812-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="eb812-111">Uwaga: Jeśli centrum administracyjnego usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być problem z usługą tymczasową.</span><span class="sxs-lookup"><span data-stu-id="eb812-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="eb812-112">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="eb812-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


