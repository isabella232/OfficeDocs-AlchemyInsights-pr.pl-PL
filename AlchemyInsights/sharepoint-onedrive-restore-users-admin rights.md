---
title: Rozwiązywanie problemów z odmowa dostępu wiadomości do OneDrive dla witryn biznesowych
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766721"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="ddce8-102">Rozwiązywanie problemów z odmowa dostępu wiadomości do OneDrive dla witryn biznesowych</span><span class="sxs-lookup"><span data-stu-id="ddce8-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="ddce8-103">Ten problem występuje najczęściej, gdy użytkownik zostanie usunięty i utworzony ponownie z tej samej głównej nazwy użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="ddce8-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ddce8-104">Nowe konto jest tworzone przy użyciu innego PUID (Passport Unique ID) wartość.</span><span class="sxs-lookup"><span data-stu-id="ddce8-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ddce8-105">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID.</span><span class="sxs-lookup"><span data-stu-id="ddce8-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ddce8-106">Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną (OU) usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddce8-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ddce8-107">Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie są przenoszone do innej jednostki organizacyjnej i resynced z programu SharePoint, mogą wystąpić ten problem.</span><span class="sxs-lookup"><span data-stu-id="ddce8-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="ddce8-108">Aby rozwiązać ten problem, należy przywrócić oryginalną nazwę UPN z krokami w artykule, [Przywróć użytkownika w pakiecie Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ddce8-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="ddce8-109">Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny OneDrive, wykonując następujące kroki, [Usuń użytkownika z listy informacji o]()użytkowniku.</span><span class="sxs-lookup"><span data-stu-id="ddce8-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="ddce8-110">Po wykonaniu tej czynności można sprawdzić, czy użytkownik ma uprawnienia administratora do witryny OneDrive, wykonując kroki, aby [dodać administratora dla użytkownika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="ddce8-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="ddce8-111">Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł, [zrozumienie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ddce8-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
