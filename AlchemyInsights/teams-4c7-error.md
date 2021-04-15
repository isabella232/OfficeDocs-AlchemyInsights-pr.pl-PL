---
title: Błąd teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786679"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="b8c9f-102">Błąd 4c7 w aplikacji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b8c9f-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="b8c9f-103">Ten błąd występuje, ponieważ aplikacja Microsoft Teams wymaga uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="b8c9f-104">Po wdrożeniu usług feder formowych Active Directory (AD FS) uwierzytelnianie formularzy nie jest domyślnie włączone w intranecie.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="b8c9f-105">Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="b8c9f-106">Aby rozwiązać ten problem, włącz uwierzytelnianie formularzy przy użyciu Microsoft Management Console AD FS (MMC) na komputerze, na którym znajduje się kopia lokalna usługi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="b8c9f-107">Aby to zrobić, wykonaj następujące kroki.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="b8c9f-108">W okienku nawigacji przejdź do strony **Zasady uwierzytelniania.**</span><span class="sxs-lookup"><span data-stu-id="b8c9f-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="b8c9f-109">W **obszarze Akcje** w okienku szczegółów wybierz pozycję Edytuj globalne **uwierzytelnianie podstawowe**.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="b8c9f-110">Na karcie **Intranet** wybierz pozycję **Uwierzytelnianie formularzy**.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="b8c9f-111">Wybierz **przycisk OK** (lub **Zastosuj).**</span><span class="sxs-lookup"><span data-stu-id="b8c9f-111">Select **OK** (or **Apply**).</span></span>