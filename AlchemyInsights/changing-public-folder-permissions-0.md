---
title: Zmienianie uprawnień do folderu publicznego
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714257"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="fb82a-102">Zmienianie uprawnień do folderu publicznego</span><span class="sxs-lookup"><span data-stu-id="fb82a-102">Changing public folder permissions</span></span>

<span data-ttu-id="fb82a-103">Uprawnienia do folderu publicznego mogą być zmieniane przez użytkowników i administratorów w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="fb82a-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="fb82a-104">Administratorzy mogą również kontrolować uprawnienia w centrum administracyjnym programu Exchange (SKK), wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="fb82a-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="fb82a-105">W centrum administracyjnym usługi Microsoft 365 **Przejdź do** \> **programu Exchange**Center Center.</span><span class="sxs-lookup"><span data-stu-id="fb82a-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="fb82a-106">Wybierz pozycję **Foldery publiczne**.</span><span class="sxs-lookup"><span data-stu-id="fb82a-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="fb82a-107">W tym miejscu możesz zmienić uprawnienia dla poszczególnych folderów publicznych, przypisując grupom zabezpieczeń uprawnienia.</span><span class="sxs-lookup"><span data-stu-id="fb82a-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="fb82a-108">Aby użytkownik końcowy mógł zmienić uprawnienia do folderu publicznego, użytkownik musi mieć prawa właściciela do tego folderu.</span><span class="sxs-lookup"><span data-stu-id="fb82a-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="fb82a-109">Postępuj zgodnie z procedurą opisaną w sekcji [diagnozowanie i rozwiązywanie problemów z uprawnieniami](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) do folderu publicznego w celu rozwiązywania problemów z uprawnieniami do folderu publicznego.</span><span class="sxs-lookup"><span data-stu-id="fb82a-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="fb82a-110">**Uwaga**: podczas próby zmiany uprawnień w folderach publicznych mogą wystąpić pewne znane problemy.</span><span class="sxs-lookup"><span data-stu-id="fb82a-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="fb82a-111">Aby uzyskać więcej informacji, zobacz następujące artykuły.</span><span class="sxs-lookup"><span data-stu-id="fb82a-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="fb82a-112">Nie można zastosować uprawnień do podfolderów folderów publicznych w centrum administracyjnym</span><span class="sxs-lookup"><span data-stu-id="fb82a-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="fb82a-113">Błąd "Skrzynka pocztowa nie została znaleziona w lesie lokalnym" podczas uzyskiwania dostępu do folderów publicznych</span><span class="sxs-lookup"><span data-stu-id="fb82a-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
