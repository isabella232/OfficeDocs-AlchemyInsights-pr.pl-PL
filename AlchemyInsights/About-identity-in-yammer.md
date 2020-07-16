---
title: Informacje o tożsamości w usłudze Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148307"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="a5ad4-102">Informacje o tożsamości w usłudze Yammer</span><span class="sxs-lookup"><span data-stu-id="a5ad4-102">About identity in Yammer</span></span>

<span data-ttu-id="a5ad4-103">Zaleca się, aby wszystkie sieci podjęła następujące kroki w celu uniknięcia problemów związanych z tożsamością:</span><span class="sxs-lookup"><span data-stu-id="a5ad4-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="a5ad4-104">Wymuszaj tożsamość usługi Office 365 po zainicjowaniu obsługi administracyjnej kont usługi Microsoft 365 dla użytkowników usługi Azure AD, aby upewnić się, że wszyscy użytkownicy logują się przy użyciu podstawowego konta usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="a5ad4-105">Aby uzyskać więcej informacji, zobacz [Wymuszanie tożsamości usługi Office 365 dla użytkowników usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="a5ad4-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="a5ad4-106">Skonsoliduj wiele sieci yammer.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="a5ad4-107">Starsze konfiguracje usługi Yammer umożliwiają podłączenie wielu sieci usługi Yammer do jednej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="a5ad4-108">Aby uzyskać więcej informacji, zobacz [Migracja sieci — konsolidacja wielu sieci usługi Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="a5ad4-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="a5ad4-109">Opcjonalnie wymuś licencjonowanie usługi Yammer, aby zablokować użytkownikom usługę Yammer, jeśli nie mają licencji.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="a5ad4-110">Aby uzyskać więcej informacji, zobacz [Zarządzanie licencjami użytkowników usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="a5ad4-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="a5ad4-111">Na koniec inspekcji listy użytkowników dla starszych sieci Yammer i zawiesić starszych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="a5ad4-112">Zaleca się zawieszenie (dezaktywację) użytkowników zamiast ich usuwania, ponieważ usunięcie jest nieodwracalne.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="a5ad4-113">Aby uzyskać więcej informacji, zobacz [Inspekcja użytkowników usługi Yammer w sieciach połączonych z usługą Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Usuwanie użytkowników](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="a5ad4-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="a5ad4-114">Konfigurując usługę Yammer przy użyciu tych kroków, możesz również skonfigurować sieć Yammer dla trybu macierzystego dla usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5ad4-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="a5ad4-115">Aby uzyskać więcej informacji, zobacz [Konfigurowanie sieci Usługi Yammer w trybie macierzystym dla usługi Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="a5ad4-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>