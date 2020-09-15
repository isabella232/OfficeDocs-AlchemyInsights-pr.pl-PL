---
title: Błąd 4c7 aplikacji Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700213"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="6abfd-102">błąd 4c7 w aplikacji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6abfd-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="6abfd-103">Ten błąd występuje, ponieważ aplikacja Microsoft Teams wymaga uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="6abfd-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="6abfd-104">Podczas wdrażania usług federacyjnych Active Directory (AD FS) uwierzytelnianie formularzy nie jest domyślnie włączone dla intranetu.</span><span class="sxs-lookup"><span data-stu-id="6abfd-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="6abfd-105">Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="6abfd-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="6abfd-106">Aby rozwiązać ten problem, Włącz uwierzytelnianie formularzy za pomocą przystawki Microsoft Management Console (MMC) programu AD FS na komputerze, na którym jest używana kopia lokalna usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6abfd-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="6abfd-107">Aby to zrobić, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="6abfd-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="6abfd-108">W okienku nawigacji przejdź do **zasad uwierzytelniania**.</span><span class="sxs-lookup"><span data-stu-id="6abfd-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="6abfd-109">W obszarze **Akcje** w okienku szczegółów wybierz pozycję **Edytuj globalne uwierzytelnianie podstawowe**.</span><span class="sxs-lookup"><span data-stu-id="6abfd-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="6abfd-110">Na karcie **intranet** wybierz pozycję **uwierzytelnianie formularzy**.</span><span class="sxs-lookup"><span data-stu-id="6abfd-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="6abfd-111">Wybierz **przycisk OK** (lub **Zastosuj**).</span><span class="sxs-lookup"><span data-stu-id="6abfd-111">Select **OK** (or **Apply**).</span></span>