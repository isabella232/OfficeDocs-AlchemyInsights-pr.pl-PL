---
title: Rozwiązywanie problemów z odmową dostępu wiadomości do witryn usługi OneDrive dla firm
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670626"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="32213-102">Rozwiązywanie problemów z odmową dostępu wiadomości do witryn usługi OneDrive dla firm</span><span class="sxs-lookup"><span data-stu-id="32213-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="32213-103">Ten problem występuje najczęściej, gdy użytkownik jest usuwany i tworzony ponownie przy użyciu tej samej głównej nazwy użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="32213-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="32213-104">Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (unikatowy identyfikator paszportu).</span><span class="sxs-lookup"><span data-stu-id="32213-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="32213-105">Gdy użytkownik usiłuje uzyskać dostęp do zbioru witryn lub jego usługi OneDrive, użytkownik ma nieprawidłowy identyfikator PUID.</span><span class="sxs-lookup"><span data-stu-id="32213-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="32213-106">Drugi scenariusz obejmuje synchronizację katalogów za pomocą jednostki organizacyjnej (OU) Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32213-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="32213-107">Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przesunięte do innej jednostki organizacyjnej i ponownie zsynchronizowane z programem SharePoint, mogą wystąpić ten problem.</span><span class="sxs-lookup"><span data-stu-id="32213-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="32213-108">Aby rozwiązać ten problem, należy przywrócić oryginalną główną nazwę użytkownika, wykonując czynności opisane w artykule, [przywracanie użytkownika w programie Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="32213-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="32213-109">Jeśli nie można przywrócić oryginalnego użytkownika, należy usunąć starego użytkownika z witryny usługi OneDrive, wykonując poniższe czynności, [a następnie usunąć użytkownika z listy informacje o użytkowniku]().</span><span class="sxs-lookup"><span data-stu-id="32213-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="32213-110">Po wykonaniu tej czynności można sprawdzić, czy użytkownik ma uprawnienia administratora witryny usługi OneDrive, wykonując kroki opisane w temacie [Dodawanie administratora do usługi OneDrive użytkownika](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="32213-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="32213-111">Aby uzyskać więcej informacji na temat poziomów uprawnień, zobacz artykuł [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="32213-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
