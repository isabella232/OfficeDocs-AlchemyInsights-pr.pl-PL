---
title: Drużyny 4c7 błąd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796280"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="fce86-102">błąd 4c7 w programie Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fce86-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="fce86-103">Ten błąd występuje, ponieważ Microsoft Teams wymaga uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="fce86-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="fce86-104">Podczas wdrażania programu Active Directory Federation Services (AD FS), uwierzytelnianie formularzy nie jest włączona dla intranetu domyślnie.</span><span class="sxs-lookup"><span data-stu-id="fce86-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="fce86-105">Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="fce86-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="fce86-106">Aby rozwiązać ten problem, należy włączyć uwierzytelnianie formularzy przy użyciu przystawki programu AD FS Microsoft Management Console (MMC) na komputerze, który ma lokalną kopię usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fce86-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="fce86-107">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="fce86-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="fce86-108">W okienku nawigacji przejdź do **zasad uwierzytelniania**.</span><span class="sxs-lookup"><span data-stu-id="fce86-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="fce86-109">W obszarze **Akcje** w okienku szczegółów wybierz opcję **Edytuj globalne uwierzytelnianie podstawowe**.</span><span class="sxs-lookup"><span data-stu-id="fce86-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="fce86-110">Na karcie **intranet** wybierz opcję **uwierzytelnianie formularzy**.</span><span class="sxs-lookup"><span data-stu-id="fce86-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="fce86-111">Wybierz **OK** (lub **Zastosuj**).</span><span class="sxs-lookup"><span data-stu-id="fce86-111">Select **OK** (or **Apply**).</span></span>