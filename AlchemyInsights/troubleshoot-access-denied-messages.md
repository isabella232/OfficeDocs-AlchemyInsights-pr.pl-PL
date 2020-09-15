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
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690793"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="967db-102">Rozwiązywanie problemów z odmową dostępu wiadomości</span><span class="sxs-lookup"><span data-stu-id="967db-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="967db-103">Jeśli ktoś otrzyma komunikat "odmowa dostępu" do folderu udostępnionego w programie SharePoint, administrator zbioru witryn może włączyć tryb blokowania uprawnień użytkownika z ograniczonym dostępem.</span><span class="sxs-lookup"><span data-stu-id="967db-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="967db-104">Aby wyłączyć tę funkcję:</span><span class="sxs-lookup"><span data-stu-id="967db-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="967db-105">Przejdź do witryny, kliknij ikonę Ustawienia, a następnie kliknij pozycję **Ustawienia witryny**.</span><span class="sxs-lookup"><span data-stu-id="967db-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="967db-106">W obszarze **Administracja zbiorem witryn**kliknij pozycję **Funkcje zbioru witryn**.</span><span class="sxs-lookup"><span data-stu-id="967db-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="967db-107">Obok pozycji **tryb blokowania uprawnień użytkownika z ograniczonym dostępem**kliknij pozycję **Dezaktywuj**.</span><span class="sxs-lookup"><span data-stu-id="967db-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="967db-108">Komunikat Odmowa dostępu może również wystąpić w przypadku folderów udostępnionych, jeśli witryna jest witryną publikowania.</span><span class="sxs-lookup"><span data-stu-id="967db-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="967db-109">Aby uzyskać informacje, zobacz [odmowa dostępu podczas uzyskiwania dostępu do folderu udostępnionego](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="967db-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="967db-110">Jeśli ktoś uzyskał komunikat "odmowa dostępu" podczas próby wyświetlenia wniosków o dostęp, użytkownik musi zostać dodany jako administrator zbioru witryn lub członek grupy Właściciele witryny.</span><span class="sxs-lookup"><span data-stu-id="967db-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="967db-111">Aby uzyskać więcej informacji, zobacz [odmowa dostępu do listy żądań dostępu](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="967db-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="967db-112">Jeśli użytkownik uzyskał komunikat "odmowa dostępu" po usunięciu go z lokalnej usługi Active Directory, a następnie ponownie dodany, zobacz [odmowa dostępu po zsynchronizowaniu konta użytkownika z systemem Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="967db-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

