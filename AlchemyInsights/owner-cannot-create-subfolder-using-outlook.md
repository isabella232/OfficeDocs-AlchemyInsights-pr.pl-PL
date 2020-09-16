---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665728"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="fc161-102">Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook</span><span class="sxs-lookup"><span data-stu-id="fc161-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="fc161-103">**W przypadku tworzenia podfolderów za pomocą programu Outlook jest już dostępny problem z właścicielami folderów publicznych. Problem zostanie wkrótce rozwiązany.**</span><span class="sxs-lookup"><span data-stu-id="fc161-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="fc161-104">W międzyczasie Użyj jednego z poniższych obejść:</span><span class="sxs-lookup"><span data-stu-id="fc161-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="fc161-105">Tworzenie podfolderu przy użyciu programu Outlook dla komputerów MAC w celu uzyskania wpływu tylko na program Outlook dla komputerów stacjonarnych (wszystkie wersje)</span><span class="sxs-lookup"><span data-stu-id="fc161-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="fc161-106">Tworzenie podfolderu przez administratora za pomocą powłoki EXO lub narzędzia SKK</span><span class="sxs-lookup"><span data-stu-id="fc161-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="fc161-107">Zmienianie DefaultPublicFolderMailbox/EffectivePublicFolderMailbox użytkownika na inną skrzynkę pocztową niż Skrzynka pocztowa zawartości folderu powodującego problem</span><span class="sxs-lookup"><span data-stu-id="fc161-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="fc161-108">*Set-Mailbox Użytkownik1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="fc161-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="fc161-109">Poczekaj na godzinę, ponownie uruchom klienta programu Outlook</span><span class="sxs-lookup"><span data-stu-id="fc161-109">Wait for an hour, restart outlook client</span></span>