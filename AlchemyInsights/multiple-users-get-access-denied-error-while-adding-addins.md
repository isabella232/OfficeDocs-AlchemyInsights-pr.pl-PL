---
title: Wielu użytkowników otrzymuje błąd odmowy dostępu podczas dodawania dodatków w programie Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424170"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="5b7c8-102">Wielu użytkowników otrzymuje błąd odmowy dostępu podczas dodawania dodatków w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="5b7c8-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="5b7c8-103">Można określić, którzy administratorzy w organizacji mają uprawnienia do instalowania dodatków programu Outlook i zarządzania nimi.</span><span class="sxs-lookup"><span data-stu-id="5b7c8-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="5b7c8-104">Można również określić, którzy użytkownicy w organizacji mają uprawnienia do instalowania dodatków i zarządzania nimi na własny użytek.</span><span class="sxs-lookup"><span data-stu-id="5b7c8-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="5b7c8-105">Aby uzyskać szczegółowe informacje, zobacz [Określanie administratorów i użytkowników, którzy mogą instalować dodatki dla programu Outlook i zarządzać nimi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="5b7c8-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="5b7c8-106">Aby sprawdzić, czy pomyślnie przypisano uprawnienia użytkownikowi, <Role Name> zastąp nazwą roli do zweryfikowania i uruchom następujące polecenie w programie Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5b7c8-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="5b7c8-107">Get-ManagementRoleAssignment -Rola " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="5b7c8-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="5b7c8-108">W tym przykładzie pokazano, jak sprawdzić, komu przypisano uprawnienia do instalowania dodatków ze Sklepu Office dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="5b7c8-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="5b7c8-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="5b7c8-109">PowerShell</span></span>

<span data-ttu-id="5b7c8-110">-Rola "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="5b7c8-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="5b7c8-111">W wynikach, Get-ManagementRoleAssignment, przejrzyj wpisy w kolumnie Skuteczni użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="5b7c8-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="5b7c8-112">Aby uzyskać szczegółowe informacje o składni i parametrach, zobacz [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="5b7c8-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 