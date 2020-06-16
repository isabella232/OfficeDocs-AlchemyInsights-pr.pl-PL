---
title: Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749140"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="0d6fd-102">Właściciel nie może utworzyć podfolderu przy użyciu programu Outlook</span><span class="sxs-lookup"><span data-stu-id="0d6fd-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="0d6fd-103">**Istnieje stały problem z właścicielami folderów publicznych tworzenia podfolderów za pomocą programu Outlook. Problem zostanie wkrótce rozwiązany.**</span><span class="sxs-lookup"><span data-stu-id="0d6fd-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="0d6fd-104">W międzyczasie należy użyć jednego z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="0d6fd-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="0d6fd-105">Tworzenie podfolderu za pomocą programu Outlook dla komputerów MAC w celu utworzenia podfolderu, ponieważ problem dotyczy tylko systemu Outlook dla komputerów stacjonarnych (wszystkie wersje)</span><span class="sxs-lookup"><span data-stu-id="0d6fd-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="0d6fd-106">Czy administrator utworzyć podfolder przy użyciu EXO Shell lub EAC</span><span class="sxs-lookup"><span data-stu-id="0d6fd-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="0d6fd-107">Zmień domyślną skrzynkę adresową folderu</span><span class="sxs-lookup"><span data-stu-id="0d6fd-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="0d6fd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="0d6fd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="0d6fd-109">Odczekanie godziny, ponowne uruchomienie klienta programu Outlook</span><span class="sxs-lookup"><span data-stu-id="0d6fd-109">Wait for an hour, restart outlook client</span></span>