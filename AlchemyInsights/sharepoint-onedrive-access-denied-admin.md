---
title: Rozwiązywanie problemów z odmową dostępu wiadomości
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767672"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="dca24-102">Rozwiązywanie problemów z odmową dostępu wiadomości w programie SharePoint/centrum administracyjnym usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="dca24-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="dca24-103">Jeśli zostanie wyświetlony komunikat Odmowa dostępu podczas próby przełączenia się do centrum administracyjnego programu SharePoint/OneDrive, upewnij się, że [użytkownik przypisał licencję użytkownikowi](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="dca24-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="dca24-104">Jeśli użytkownik ma licencję, należy również upewnić się, że jest [mu przypisana rola administratora](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , która może uzyskać dostęp do centrów administracyjnych.</span><span class="sxs-lookup"><span data-stu-id="dca24-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="dca24-105">Ten problem może również wystąpić, gdy użytkownik jest usuwany i tworzony ponownie przy użyciu tej samej głównej nazwy użytkownika (UPN).</span><span class="sxs-lookup"><span data-stu-id="dca24-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="dca24-106">Nowe konto jest tworzone przy użyciu innej wartości identyfikatora PUID (unikatowy identyfikator paszportu).</span><span class="sxs-lookup"><span data-stu-id="dca24-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="dca24-107">Gdy użytkownik usiłuje uzyskać dostęp do zbioru witryn lub jego usługi OneDrive, użytkownik ma nieprawidłowy identyfikator PUID.</span><span class="sxs-lookup"><span data-stu-id="dca24-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="dca24-108">Drugi scenariusz obejmuje synchronizację katalogów za pomocą jednostki organizacyjnej (OU) Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dca24-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="dca24-109">Jeśli użytkownicy już zalogowali się do programu SharePoint, a następnie zostaną przesunięte do innej jednostki organizacyjnej i ponownie zsynchronizowane z programem SharePoint, mogą wystąpić ten problem.</span><span class="sxs-lookup"><span data-stu-id="dca24-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="dca24-110">Aby rozwiązać ten problem, należy przywrócić oryginalną główną nazwę użytkownika, wykonując czynności opisane w artykule, [przywracanie użytkownika w programie Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="dca24-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="dca24-111">Uwaga: Jeśli centrum administracyjne usługi OneDrive lub programu SharePoint nie jest dostępne dla wielu użytkowników, którzy wcześniej mieli dostęp, może to być tymczasowy problem z usługą.</span><span class="sxs-lookup"><span data-stu-id="dca24-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="dca24-112">[Sprawdź pulpit nawigacyjny kondycji usługi](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="dca24-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


