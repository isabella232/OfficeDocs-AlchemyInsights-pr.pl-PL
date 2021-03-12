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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704904"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d9fa6-102">Rozwiązywanie problemów z wiadomościami o odmowie dostępu</span><span class="sxs-lookup"><span data-stu-id="d9fa6-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d9fa6-103">Jeśli ktoś otrzymał komunikat "Odmowa dostępu" do folderu udostępnionego w programie SharePoint, administrator zbioru witryn mógł włączyć "Tryb blokowania uprawnień użytkownika z ograniczonym dostępem".</span><span class="sxs-lookup"><span data-stu-id="d9fa6-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d9fa6-104">Aby wyłączyć tę wyłączyć:</span><span class="sxs-lookup"><span data-stu-id="d9fa6-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d9fa6-105">Przejdź do witryny, kliknij ikonę Ustawienia, a następnie kliknij **pozycję Ustawienia witryny.**</span><span class="sxs-lookup"><span data-stu-id="d9fa6-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d9fa6-106">W **obszarze Administracja zbiorem witryn** kliknij pozycję Funkcje zbioru **witryn.**</span><span class="sxs-lookup"><span data-stu-id="d9fa6-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d9fa6-107">Obok trybu **blokowania uprawnień** użytkownika z ograniczonym dostępem kliknij pozycję **Dezaktywuj.**</span><span class="sxs-lookup"><span data-stu-id="d9fa6-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d9fa6-108">Komunikat o odmowie dostępu może również wystąpić w przypadku folderów udostępnionych, jeśli witryna jest witryną publikowania.</span><span class="sxs-lookup"><span data-stu-id="d9fa6-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d9fa6-109">Aby uzyskać informacje, zobacz ["Odmowa dostępu podczas uzyskiwania dostępu do folderu udostępnionego".](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="d9fa6-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="d9fa6-110">Jeśli podczas próby wyświetlenia żądań dostępu ktoś otrzymał komunikat "Odmowa dostępu", należy dodać tego użytkownika jako administratora zbioru witryn lub członka grupy Właściciele witryny.</span><span class="sxs-lookup"><span data-stu-id="d9fa6-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d9fa6-111">Aby uzyskać więcej informacji, zobacz listę Żądań dostępu [odrzuconych dostępu.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="d9fa6-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d9fa6-112">Jeśli użytkownik otrzymał komunikat "Odmowa dostępu" po usunięciu go z lokalnej usługi Active Directory, a następnie dodaniu go z powrotem, zobacz "Odmowa dostępu, gdy konto użytkownika jest synchronizowane z platformą [Microsoft 365".](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="d9fa6-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

