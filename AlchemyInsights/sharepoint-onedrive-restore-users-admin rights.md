---
title: Rozwiązywanie problemów z dostępem odmowa wiadomości do OneDrive dla witryn biznesu
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223434"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="575e1-102">Rozwiązywanie problemów z dostępem odmowa wiadomości do OneDrive dla witryn biznesu</span><span class="sxs-lookup"><span data-stu-id="575e1-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="575e1-103">Ten problem najczęściej występuje, gdy użytkownik jest usunięty i utworzony ponownie z samą główną nazwę użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="575e1-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="575e1-104">Nowe konto jest tworzone przy użyciu różnych wartości PUID (unikatowy identyfikator usługi Passport).</span><span class="sxs-lookup"><span data-stu-id="575e1-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="575e1-105">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub ich OneDrive, użytkownik ma niepoprawne PUID.</span><span class="sxs-lookup"><span data-stu-id="575e1-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="575e1-106">Drugi scenariusz obejmuje synchronizacji katalogów z jednostki organizacyjnej (OU) usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="575e1-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="575e1-107">Jeśli użytkownicy mają już zarejestrowany w programie SharePoint, a następnie są przenoszone do innej jednostki Organizacyjnej i resynced z programem SharePoint, mogą oni napotkać ten problem.</span><span class="sxs-lookup"><span data-stu-id="575e1-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="575e1-108">Aby rozwiązać ten problem, należy przywrócić oryginalny UPN czynności opisanych w artykule,[przywracania przez użytkownika w usłudze Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="575e1-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="575e1-109">Po tej czynności można sprawdzić, czy użytkownik posiada uprawnienia administratora do witryny OneDrive przez wykonanie kroków do [administratora Dodaj użytkownika dla użytkownika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="575e1-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="575e1-110">Aby uzyskać więcej informacji dotyczących poziomów uprawnień zobacz artykuł, [Opis poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="575e1-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
