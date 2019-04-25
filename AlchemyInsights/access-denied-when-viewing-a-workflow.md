---
title: Odmowa dostępu podczas przeglądania przepływu pracy
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389897"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="bc93c-102">Odmowa dostępu podczas przeglądania przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="bc93c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="bc93c-103">2013 przepływów pracy programu SharePoint, która próbuje wysłać wiadomość e-mail do grupy programu SharePoint może się niepowodzeniem z komunikatem o błędzie "Odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawiona dla wszystkich.</span><span class="sxs-lookup"><span data-stu-id="bc93c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="bc93c-104">**Aby rozwiązać ten problem, wykonaj następujące kroki:**</span><span class="sxs-lookup"><span data-stu-id="bc93c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="bc93c-105">Zezwalaj wszystkim zobaczyć członków grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bc93c-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="bc93c-106">Usuń grupę programu SharePoint z do lub DW wiersz wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="bc93c-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="bc93c-107">Jawnie dodać użytkowników do do lub DW linii, jeśli nie można zmienić widoczności członkostwa grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bc93c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="bc93c-108">Aby wyświetlić więcej szczegółów można znaleźć [HTTP ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)nieuprawnione do /_vti_bin/client.svc/sp.utilities.utility.SendEmail.</span><span class="sxs-lookup"><span data-stu-id="bc93c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

