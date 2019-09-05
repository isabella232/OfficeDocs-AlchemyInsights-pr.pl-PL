---
title: Włącz inspekcję skrzynek pocztowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736263"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="54d94-102">Włącz inspekcję skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="54d94-102">Enable mailbox auditing</span></span>

<span data-ttu-id="54d94-103">Aby włączyć inspekcję skrzynek pocztowych dla jednego użytkownika lub całej organizacji, należy uruchomić następujące polecenia cmdlet z zdalnej powłoki zasilania:</span><span class="sxs-lookup"><span data-stu-id="54d94-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="54d94-104">**Pojedynczy użytkownik**</span><span class="sxs-lookup"><span data-stu-id="54d94-104">**Single User**</span></span>
  
<span data-ttu-id="54d94-105">Zestaw-Mailbox-tożsamość "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="54d94-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="54d94-106">**Organizacji**</span><span class="sxs-lookup"><span data-stu-id="54d94-106">**Organization**</span></span>
  
<span data-ttu-id="54d94-107">Pobierz skrzynki pocztowej-ResultSize nieograniczony-filtr {RecipientTypeDetails-EQ "UserMailbox"} | $true AuditEnabled zestawu skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="54d94-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="54d94-108">Dowiedz się więcej</span><span class="sxs-lookup"><span data-stu-id="54d94-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

