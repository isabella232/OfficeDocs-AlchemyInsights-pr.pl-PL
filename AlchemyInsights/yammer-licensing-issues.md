---
title: Problemy z licencjonowaniem usługi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657286"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="dece2-102">Problemy z licencjonowaniem usługi Yammer</span><span class="sxs-lookup"><span data-stu-id="dece2-102">Yammer licensing issues</span></span>

<span data-ttu-id="dece2-103">Wszyscy użytkownicy muszą mieć licencję na korzystanie z usługi Yammer Enterprise, ale domyślnie usługa Yammer nie wymaga posiadania licencji na dostęp do usługi.</span><span class="sxs-lookup"><span data-stu-id="dece2-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="dece2-104">Gdy administrator zmieni ustawienie w celu zablokowania użytkowników programu Microsoft 365 bez licencji usługi Yammer, użytkownicy, którym nie przypisano licencji usługi Yammer Enterprise, mogą uzyskać dostęp do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="dece2-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="dece2-105">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w pakiecie Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="dece2-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="dece2-106">Po usunięciu licencji od użytkowników kafelek usługi Yammer nie jest już wyświetlany, a inne usługi mogą używać usuwania licencji w celu ukrycia funkcji.</span><span class="sxs-lookup"><span data-stu-id="dece2-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="dece2-107">W innych przypadkach nadal mogą być wyświetlane funkcje, ale wymagane jest przypisanie licencji.</span><span class="sxs-lookup"><span data-stu-id="dece2-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="dece2-108">**Licencja nie jest aktualizowana dla użytkownika**</span><span class="sxs-lookup"><span data-stu-id="dece2-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="dece2-109">Czasami użytkownik ma przypisaną licencję, ale nadal nie może uzyskać dostępu do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="dece2-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="dece2-110">Prawdopodobieństwo wystąpienia opóźnień jest większe, gdy trwa przydział licencji masowej.</span><span class="sxs-lookup"><span data-stu-id="dece2-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="dece2-111">Użytkownicy usługi Yammer mogą nie zostać zaktualizowani w takiej samej kolejności, w jakiej licencje są zmieniane w usłudze Azure AD, ponieważ system jest uruchamiany asynchronicznie.</span><span class="sxs-lookup"><span data-stu-id="dece2-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="dece2-112">Poczekaj na 24 godziny przed otwarciem sprawy pomocy technicznej, aby raportować problemy z synchronizacją licencji.</span><span class="sxs-lookup"><span data-stu-id="dece2-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="dece2-113">**Przydział licencji zbiorczej**</span><span class="sxs-lookup"><span data-stu-id="dece2-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="dece2-114">Licencje można przypisywać za pośrednictwem Centrum administracyjnego lub skryptów programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dece2-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="dece2-115">Aby uzyskać więcej informacji, zobacz [Przypisywanie licencji do użytkowników](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Przypisywanie licencji do kont użytkowników przy użyciu programu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="dece2-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="dece2-116">Pomoc techniczna firmy Microsoft nie zapewnia pomocy w tworzeniu skryptów, ale dostępna jest dokumentacja dotycząca przydziału licencji usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="dece2-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="dece2-117">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami usługi Yammer za pomocą programu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="dece2-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>