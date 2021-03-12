---
title: Rozwiązywanie problemów z wiadomościami o odmowie dostępu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707964"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="1d531-102">Rozwiązywanie problemów z komunikatami o odmowie dostępu w centrum administracyjnym programu SharePoint/usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="1d531-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="1d531-103">Jeśli podczas próby przeglądania centrum administracyjnego programu SharePoint/usługi OneDrive jest wyświetlany komunikat o odmowie dostępu, upewnij się, że przypisano licencję [do użytkownika.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="1d531-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="1d531-104">Jeśli użytkownik ma licencję, należy również upewnić się, że ma przypisaną rolę [administratora,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) która może uzyskać dostęp do centrów aadministracyjnym.</span><span class="sxs-lookup"><span data-stu-id="1d531-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="1d531-105">Ten problem może również wystąpić, gdy użytkownik zostanie usunięty i utworzony ponownie z tą samą główną nazwą użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="1d531-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="1d531-106">Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="1d531-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="1d531-107">Gdy użytkownik próbuje uzyskać dostęp do zbioru witryn lub usługi OneDrive, ma on nieprawidłowy identyfikator PUID.</span><span class="sxs-lookup"><span data-stu-id="1d531-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="1d531-108">Drugi scenariusz obejmuje synchronizację katalogów z jednostką organizacyjną usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1d531-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="1d531-109">Ten problem może wystąpić, jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostali przeniesioni do innej społeczności użytkownika i ponownie zsynchroniznini z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d531-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="1d531-110">Aby rozwiązać ten problem, przywróć pierwotną nazwę upn zgodnie z instrukcjami w artykule Przywróć użytkownika na platformie [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="1d531-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="1d531-111">Uwaga: Jeśli centrum administracyjne usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może wystąpić tymczasowy problem z usługą.</span><span class="sxs-lookup"><span data-stu-id="1d531-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="1d531-112">[Sprawdź pulpit nawigacyjny kondycji usługi.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="1d531-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


