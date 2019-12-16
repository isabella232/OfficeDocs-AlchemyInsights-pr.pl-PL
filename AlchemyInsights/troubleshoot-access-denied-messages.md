---
title: Rozwiązywanie problemów z komunikatami odmowa dostępu
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050715"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="194b1-102">Rozwiązywanie problemów z komunikatami odmowa dostępu</span><span class="sxs-lookup"><span data-stu-id="194b1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="194b1-103">Jeśli ktoś dostał komunikat "odmowa dostępu" do folderu udostępnionego w programie SharePoint, administrator zbioru witryn może mieć włączone "ograniczony dostęp użytkownika tryb blokowania uprawnień."</span><span class="sxs-lookup"><span data-stu-id="194b1-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="194b1-104">Aby wyłączyć tę funkcję:</span><span class="sxs-lookup"><span data-stu-id="194b1-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="194b1-105">Przejdź do witryny, kliknij ikonę Ustawienia, a następnie kliknij przycisk **Ustawienia witryny**.</span><span class="sxs-lookup"><span data-stu-id="194b1-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="194b1-106">W obszarze **Administracja zbioru witryn**kliknij pozycję **Funkcje zbioru witryn**.</span><span class="sxs-lookup"><span data-stu-id="194b1-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="194b1-107">Obok **ograniczonego dostępu do trybu blokowania uprawnień użytkownika**kliknij przycisk **Dezaktywuj**.</span><span class="sxs-lookup"><span data-stu-id="194b1-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="194b1-108">Komunikat Odmowa dostępu może również wystąpić dla folderów udostępnionych, jeśli witryna jest witryną publikowania.</span><span class="sxs-lookup"><span data-stu-id="194b1-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="194b1-109">Aby uzyskać informacje, zobacz [odmowa dostępu podczas uzyskiwania dostępu do folderu udostępnionego](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="194b1-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="194b1-110">Jeśli ktoś dostał komunikat "odmowa dostępu" podczas próby wyświetlenia żądania dostępu, użytkownik musi zostać dodany jako administrator zbioru witryn lub członek grupy właścicieli dla witryny.</span><span class="sxs-lookup"><span data-stu-id="194b1-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="194b1-111">Aby uzyskać więcej informacji, zobacz [listy odmowa dostępu do żądań dostępu](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="194b1-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="194b1-112">Jeśli użytkownik dostał komunikat "odmowa dostępu" po zostały usunięte z lokalnej usługi Active Directory, a następnie dodane wstecz, zobacz [odmowa dostępu, gdy konto użytkownika jest synchronizowane z pakietem Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="194b1-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

