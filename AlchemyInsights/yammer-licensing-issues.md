---
title: Problemy z licencjonowaniem usługi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148316"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="19067-102">Problemy z licencjonowaniem usługi Yammer</span><span class="sxs-lookup"><span data-stu-id="19067-102">Yammer licensing issues</span></span>

<span data-ttu-id="19067-103">Wszyscy użytkownicy muszą mieć licencję na korzystanie z usługi Yammer Enterprise, ale domyślnie usługa Yammer nie wymaga od użytkowników licencji na dostęp do usługi.</span><span class="sxs-lookup"><span data-stu-id="19067-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="19067-104">Gdy administrator zmieni to ustawienie, aby zablokować użytkowników usługi Microsoft 365 bez licencji Yammer, użytkownicy, którym nie przypisano licencji Yammer Enterprise, nie mogą uzyskać dostępu do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="19067-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="19067-105">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="19067-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="19067-106">Gdy licencje są usuwane z użytkowników, kafelek Yammer nie jest już wyświetlany, a inne usługi mogą używać usuwania licencji do ukrywania funkcji.</span><span class="sxs-lookup"><span data-stu-id="19067-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="19067-107">W innych przypadkach funkcje mogą nadal pojawiać się, ale wymagają przypisania licencji do działania.</span><span class="sxs-lookup"><span data-stu-id="19067-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="19067-108">**Licencja nie jest aktualizowana dla użytkownika**</span><span class="sxs-lookup"><span data-stu-id="19067-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="19067-109">Od czasu do czasu użytkownikowi jest przypisywana licencja, ale nadal nie może uzyskać dostępu do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="19067-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="19067-110">Opóźnienia są bardziej prawdopodobne, gdy trwa przypisanie licencji masowej.</span><span class="sxs-lookup"><span data-stu-id="19067-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="19067-111">Użytkownicy usługi Yammer mogą nie być aktualizowane w tej samej kolejności, jak licencje są zmieniane w usłudze Azure AD, ponieważ system działa asynchronicznie.</span><span class="sxs-lookup"><span data-stu-id="19067-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="19067-112">Poczekaj do 24 godzin przed otwarciem sprawy pomocy technicznej, aby zgłosić problemy z synchronizacją licencji.</span><span class="sxs-lookup"><span data-stu-id="19067-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="19067-113">**Zbiorcze przydzielanie licencji**</span><span class="sxs-lookup"><span data-stu-id="19067-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="19067-114">Licencje można przypisać za pośrednictwem centrum administracyjnego lub skryptów programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="19067-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="19067-115">Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji użytkownikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Przypisywanie licencji do kont użytkowników w usłudze Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="19067-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="19067-116">Pomoc techniczna firmy Microsoft nie zapewnia pomocy w tworzeniu skryptów, ale dostępna jest dokumentacja dotycząca przypisywania licencji usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="19067-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="19067-117">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami usługi Yammer przy użyciu programu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="19067-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>