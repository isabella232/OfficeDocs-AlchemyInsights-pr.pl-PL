---
title: Rozwiązywanie problemów z wiadomościami odmowy dostępu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759810"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ab76d-102">Rozwiązywanie problemów z wiadomościami odmowy dostępu</span><span class="sxs-lookup"><span data-stu-id="ab76d-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ab76d-103">Jeśli ktoś otrzymał komunikat "Odmowa dostępu" do folderu udostępnionego w programie SharePoint, administrator zbioru witryn mógł włączyć "Tryb blokowania uprawnień użytkownika o ograniczonym dostępie".</span><span class="sxs-lookup"><span data-stu-id="ab76d-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ab76d-104">Aby wyłączyć tę funkcję:</span><span class="sxs-lookup"><span data-stu-id="ab76d-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ab76d-105">Przejdź do witryny, kliknij ikonę Ustawienia, a następnie kliknij pozycję **Ustawienia witryny**.</span><span class="sxs-lookup"><span data-stu-id="ab76d-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ab76d-106">W obszarze **Administracja zbiorem witryn**kliknij pozycję **Funkcje zbioru witryn**.</span><span class="sxs-lookup"><span data-stu-id="ab76d-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ab76d-107">Obok pozycji **Tryb blokowania uprawnień użytkownika o ograniczonym dostępie**kliknij pozycję **Dezaktywuj**.</span><span class="sxs-lookup"><span data-stu-id="ab76d-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ab76d-108">Komunikat odmowy dostępu może również wystąpić w przypadku folderów udostępnionych, jeśli witryna jest witryną publikowania.</span><span class="sxs-lookup"><span data-stu-id="ab76d-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ab76d-109">Aby uzyskać szczegółowe informacje, zobacz [Odmowa dostępu podczas uzyskiwania dostępu do folderu udostępnionego](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ab76d-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ab76d-110">Jeśli ktoś otrzymał komunikat "Odmowa dostępu" podczas próby wyświetlenia żądań dostępu, użytkownik musi zostać dodany jako administrator zbioru witryn lub członek grupy Właściciele witryny.</span><span class="sxs-lookup"><span data-stu-id="ab76d-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ab76d-111">Aby uzyskać więcej informacji, zobacz [Lista Odmowa dostępu do żądań dostępu](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ab76d-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ab76d-112">Jeśli użytkownik otrzymał komunikat "Odmowa dostępu" po usunięciu z usługi Active Directory w środowisku lokalnym, a następnie dodaniu z powrotem, zobacz [Odmowa dostępu, gdy konto użytkownika jest synchronizowane z usługą Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ab76d-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

