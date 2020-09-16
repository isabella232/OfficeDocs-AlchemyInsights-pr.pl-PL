---
title: Informacje o tożsamości w usłudze Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664180"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="4b82a-102">Informacje o tożsamości w usłudze Yammer</span><span class="sxs-lookup"><span data-stu-id="4b82a-102">About identity in Yammer</span></span>

<span data-ttu-id="4b82a-103">Zaleca się, aby w celu uniknięcia problemów związanych z tożsamością wszystkie sieci miały następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="4b82a-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="4b82a-104">Wymuś tożsamość pakietu Office 365 po zainicjowaniu obsługi kont Microsoft 365 dla użytkowników w usłudze Azure AD, aby upewnić się, że wszyscy użytkownicy logują się przy użyciu ich podstawowego konta Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b82a-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="4b82a-105">Aby uzyskać więcej informacji, zobacz [Wymuszaj tożsamość pakietu Office 365 dla użytkowników usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="4b82a-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="4b82a-106">Konsolidowanie wielu sieci usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="4b82a-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="4b82a-107">Starsze konfiguracje usługi Yammer umożliwiają połączenie wielu sieci Yammer z jedną dzierżawą.</span><span class="sxs-lookup"><span data-stu-id="4b82a-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="4b82a-108">Aby uzyskać więcej informacji, zobacz [Migrowanie sieci — konsolidowanie wielu sieci usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="4b82a-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="4b82a-109">Opcjonalnie Wymuś Licencjonowanie w usłudze Yammer, aby blokować użytkowników z usługi Yammer, jeśli nie mają licencji.</span><span class="sxs-lookup"><span data-stu-id="4b82a-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="4b82a-110">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w pakiecie Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4b82a-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="4b82a-111">Na koniec Przeprowadź inspekcję listy użytkowników dla starszych sieci usługi Yammer i Zawieś starszych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="4b82a-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="4b82a-112">Zaleca się, aby zamiast usuwać użytkowników zawiesić (dezaktywować), ponieważ usunięcie jest nieodwracalne.</span><span class="sxs-lookup"><span data-stu-id="4b82a-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="4b82a-113">Aby uzyskać więcej informacji, zobacz [Przeprowadź inspekcję użytkowników usługi Yammer w sieciach połączonych z pakietem Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Usuń użytkowników](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="4b82a-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="4b82a-114">Konfigurując usługę Yammer za pomocą tych kroków, możesz również skonfigurować sieć usługi Yammer dla trybu macierzystego programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b82a-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="4b82a-115">Aby uzyskać więcej informacji, zobacz [Konfigurowanie sieci usługi Yammer dla trybu macierzystego dla programu Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="4b82a-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>