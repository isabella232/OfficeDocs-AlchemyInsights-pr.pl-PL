---
title: Rozwiązywanie problemów z odmową dostępu do wiadomości do witryn usługi OneDrive dla Firm
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511194"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="b3574-102">Rozwiązywanie problemów z odmową dostępu do wiadomości do witryn usługi OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="b3574-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="b3574-103">Ten problem najczęściej występuje, gdy użytkownik jest usuwany i ponownie tworzony przy tej samej głównej nazwie użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="b3574-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b3574-104">Nowe konto jest tworzone przy użyciu innej wartości PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="b3574-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b3574-105">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawny PUID.</span><span class="sxs-lookup"><span data-stu-id="b3574-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b3574-106">Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory.A second scenario involves directory synchronizacji with an Active Directory organizational unit (OU).</span><span class="sxs-lookup"><span data-stu-id="b3574-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b3574-107">Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przeniesieni do innej usługi organizacyjnej i ponownie zsynchronizowani za pomocą programu SharePoint, może wystąpić ten problem.</span><span class="sxs-lookup"><span data-stu-id="b3574-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="b3574-108">Aby rozwiązać ten problem, należy przywrócić oryginalną nazwy UPN z krokami opisanymi w artykule, [Przywróć użytkownika w usłudze Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="b3574-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="b3574-109">Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny usługi OneDrive, wykonując te kroki, [Usuń użytkownika z listy informacji o użytkowniku]().</span><span class="sxs-lookup"><span data-stu-id="b3574-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="b3574-110">Po wykonaniu tej czynności możesz sprawdzić, czy użytkownik ma prawa administratora do witryny usługi OneDrive, wykonując kroki, aby [dodać administratora dla usługi OneDrive użytkownika](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="b3574-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="b3574-111">Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b3574-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
