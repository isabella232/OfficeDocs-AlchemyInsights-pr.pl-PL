---
title: Usuwanie osieroconego użytkownika z serwera lokalnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198592"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="cbce7-102">Usuwanie osieroconego użytkownika z serwera lokalnego</span><span class="sxs-lookup"><span data-stu-id="cbce7-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="cbce7-103">Aby usunąć osieroconego użytkownika, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="cbce7-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="cbce7-104">Wymusić synchronizację katalogów, postępując zgodnie z instrukcjami w [obszarze Co to jest tożsamość hybrydowa z usługą Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="cbce7-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="cbce7-105">Aby zweryfikować synchronizację katalogów, zobacz [Co to jest tożsamość hybrydowa z usługą Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="cbce7-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="cbce7-106">Jeśli synchronizacja działa poprawnie, ale usunięcie obiektu usługi Active Directory nie jest propagowane do usługi Azure AD, ręcznie usuń oddzielony obiekt przy użyciu jednego z następujących poleceń cmdlet usługi Azure Active Directory dla programu Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cbce7-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="cbce7-107">Usuń-MsolContaktact</span><span class="sxs-lookup"><span data-stu-id="cbce7-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="cbce7-108">Usuń-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="cbce7-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="cbce7-109">Usuń-MsolUser</span><span class="sxs-lookup"><span data-stu-id="cbce7-109">Remove-MsolUser</span></span>

    <span data-ttu-id="cbce7-110">Na przykład, aby usunąć osierocony identyfikator użytkownika john.smith@contoso.com, pierwotnie utworzony przy użyciu synchronizacji katalogów, uruchom polecenie cmdlet:</span><span class="sxs-lookup"><span data-stu-id="cbce7-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="cbce7-111">Usuń-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="cbce7-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>