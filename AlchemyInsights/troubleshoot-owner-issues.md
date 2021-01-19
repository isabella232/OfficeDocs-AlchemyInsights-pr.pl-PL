---
title: Rozwiązywanie problemów z właścicielem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901282"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="1f9f1-102">Rozwiązywanie problemów z właścicielem</span><span class="sxs-lookup"><span data-stu-id="1f9f1-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="1f9f1-103">Aby rozwiązać problemy związane ze właścicielami, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="1f9f1-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="1f9f1-104">[Dodawanie lub zmienianie administratorów subskrypcji platformy Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): grupy usługi Azure Active Directory (Azure AD) są własnością i są zarządzane przez właścicieli grupy.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="1f9f1-105">Właściciele grupy mogą być użytkownikami lub podmiotami głównymi usług i mogą zarządzać grupą, w tym członkostwem.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="1f9f1-106">Właściciele grupy mogą przypisywać tylko istniejący właściciele grupy lub Administratorzy grupy.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="1f9f1-107">Właściciele grupy nie muszą być członkami grupy.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="1f9f1-108">[Dodawanie lub zmienianie administratorów subskrypcji platformy Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): w tym artykule opisano, jak dodać lub zmienić rolę administratora dla użytkownika przy użyciu funkcji Azure RBAC w zakresie abonamentu.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="1f9f1-109">Dodaj właściciela grupy lub właściciela aplikacji za pomocą programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-109">Use PowerShell to add a group owner or an application owner.</span></span>
