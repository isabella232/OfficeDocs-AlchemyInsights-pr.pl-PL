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
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760350"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c1b7b-102">Rozwiązywanie problemów z wiadomościami odmowa dostępu w Centrum administracyjnego programu Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="c1b7b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c1b7b-103">Jeśli otrzymujesz podczas próby przejdź do Centrum administracyjnego programu Sharepoint/OneDrive komunikat o odmowie dostępu, upewnij się, że możesz [przypisać jedną licencję do użytkownika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c1b7b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="c1b7b-104">Jeśli użytkownik ma licencję, należy również upewnij się, że są one [przypisaną rolę administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) można uzyskać dostęp do centrów admin.</span><span class="sxs-lookup"><span data-stu-id="c1b7b-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="c1b7b-105">Ten problem może również wystąpić, gdy użytkownik jest usunięty i utworzony ponownie z samą główną nazwę użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="c1b7b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c1b7b-106">Nowe konto jest tworzone przy użyciu różnych wartości PUID (unikatowy identyfikator usługi Passport).</span><span class="sxs-lookup"><span data-stu-id="c1b7b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c1b7b-107">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawne PUID.</span><span class="sxs-lookup"><span data-stu-id="c1b7b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c1b7b-108">Drugi scenariusz obejmuje synchronizacji katalogów z jednostki organizacyjnej (OU) usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1b7b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c1b7b-109">Jeśli użytkownicy mają już zarejestrowany w programie SharePoint, a następnie są przenoszone do innej jednostki Organizacyjnej i resynced z programem SharePoint, mogą oni napotkać ten problem.</span><span class="sxs-lookup"><span data-stu-id="c1b7b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c1b7b-110">Aby rozwiązać ten problem, należy przywrócić oryginalny UPN czynności opisanych w artykule, [przywracania przez użytkownika w usłudze Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c1b7b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="c1b7b-111">Uwaga: Jeśli Centrum OneDrive lub administracji programu SharePoint nie jest dostępne dla wielu użytkowników, którzy uprzednio uzyskiwała dostęp, może istnieć problem tymczasowej usługi.</span><span class="sxs-lookup"><span data-stu-id="c1b7b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c1b7b-112">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c1b7b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


