---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836145"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="72264-102">Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook</span><span class="sxs-lookup"><span data-stu-id="72264-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="72264-103">**Istnieje bieżący problem z utworzeniem podfolderów przez właścicieli folderów publicznych przy użyciu programu Outlook. Ten problem zostanie wkrótce rozwiązany.**</span><span class="sxs-lookup"><span data-stu-id="72264-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="72264-104">W międzyczasie możesz skorzystać z jednego z następujących obejść:</span><span class="sxs-lookup"><span data-stu-id="72264-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="72264-105">Utwórz podfolder za pomocą programu Outlook dla komputerów Mac, ponieważ ten problem występuje tylko w programie Outlook dla komputerów stacjonarnych (wszystkie wersje)</span><span class="sxs-lookup"><span data-stu-id="72264-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="72264-106">Zleć administratorowi utworzenie podfolderu przy użyciu powłoki EXO lub Centrum administracyjnego programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="72264-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="72264-107">Zmienianie folderu DefaultPublicFolderMailbox/EffectivePublicFolderMailbox w użytkowniku na inną skrzynkę pocztową niż skrzynka pocztowa zawartości folderu powodującego problem</span><span class="sxs-lookup"><span data-stu-id="72264-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="72264-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="72264-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="72264-109">Odczekaj godzinę, uruchom ponownie klienta programu Outlook</span><span class="sxs-lookup"><span data-stu-id="72264-109">Wait for an hour, restart outlook client</span></span>