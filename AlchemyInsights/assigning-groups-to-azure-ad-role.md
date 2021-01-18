---
title: Przypisywanie grup do roli usługi Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885393"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="3b992-102">Przypisywanie grup do roli usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="3b992-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="3b992-103">Aby przypisać grupę usługi Azure AD za pomocą źródła uprawnień w usłudze Azure AD do roli usługi Azure AD, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="3b992-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="3b992-104">Utwórz nową grupę — aby utworzyć nową grupę:</span><span class="sxs-lookup"><span data-stu-id="3b992-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="3b992-105">a.</span><span class="sxs-lookup"><span data-stu-id="3b992-105">a.</span></span> <span data-ttu-id="3b992-106">Zaloguj się do centrum administracyjnego usługi Azure AD z uprawnieniami **administratora roli uprzywilejowanych** lub **administratora globalnego** .</span><span class="sxs-lookup"><span data-stu-id="3b992-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="3b992-107">b.</span><span class="sxs-lookup"><span data-stu-id="3b992-107">b.</span></span> <span data-ttu-id="3b992-108">Wybierz pozycję **grupy usługi Azure Active Directory >, > wszystkie grupy > Nowa grupa**.</span><span class="sxs-lookup"><span data-stu-id="3b992-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="3b992-109">c.</span><span class="sxs-lookup"><span data-stu-id="3b992-109">c.</span></span> <span data-ttu-id="3b992-110">Utwórz grupę.</span><span class="sxs-lookup"><span data-stu-id="3b992-110">Create the group.</span></span>

2. <span data-ttu-id="3b992-111">Przypisz rolę do grupy podczas tworzenia grupy lub po utworzeniu grupy.</span><span class="sxs-lookup"><span data-stu-id="3b992-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="3b992-112">a.</span><span class="sxs-lookup"><span data-stu-id="3b992-112">a.</span></span> <span data-ttu-id="3b992-113">Aby przypisać rolę do grupy w momencie tworzenia grupy, przełącz się na pozycję Przełącz **role usługi Azure AD do grupy** i Utwórz grupę.</span><span class="sxs-lookup"><span data-stu-id="3b992-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="3b992-114">b.</span><span class="sxs-lookup"><span data-stu-id="3b992-114">b.</span></span> <span data-ttu-id="3b992-115">Aby przypisać rolę do grupy po jej utworzeniu, przejdź do karty **przypisane role** dla nowo utworzonej grupy i przypisz tę rolę grupie.</span><span class="sxs-lookup"><span data-stu-id="3b992-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="3b992-116">**Zarządzanie członkostwem w grupie przypisanej do roli usługi Azure AD**</span><span class="sxs-lookup"><span data-stu-id="3b992-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="3b992-117">Aby zapobiec podnoszeniu uprawnień, domyślnie tylko Administratorzy ról uprzywilejowanych i Administratorzy globalni mogą modyfikować członkostwo grupy przypisanej do roli.</span><span class="sxs-lookup"><span data-stu-id="3b992-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="3b992-118">Może jednak zdecydować o przypisaniu właściciela takiej grupy i delegować to zadanie.</span><span class="sxs-lookup"><span data-stu-id="3b992-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="3b992-119">Aby uzyskać więcej informacji na temat przypisywania grup w chmurze do ról usługi Azure AD, zobacz [Przypisywanie ról usługi AD do grupy chmury](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="3b992-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="3b992-120">Aby uzyskać więcej informacji na temat rozwiązywania problemów z rolami przypisanymi do grup chmury, zobacz [Rozwiązywanie problemów z rolami przypisanymi do grup chmury](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="3b992-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





