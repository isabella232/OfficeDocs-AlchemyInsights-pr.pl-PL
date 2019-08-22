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
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495833"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d9f7d-102">Odmowa dostępu podczas przeglądania przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="d9f7d-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d9f7d-103">2013 przepływów pracy programu SharePoint, która próbuje wysłać wiadomość e-mail do grupy programu SharePoint może się niepowodzeniem z komunikatem o błędzie "Odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawiona dla wszystkich.</span><span class="sxs-lookup"><span data-stu-id="d9f7d-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d9f7d-104">**Aby rozwiązać ten problem, wykonaj następujące kroki:**</span><span class="sxs-lookup"><span data-stu-id="d9f7d-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d9f7d-105">Zezwalaj wszystkim zobaczyć członków grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d9f7d-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="d9f7d-106">Usuń grupę programu SharePoint z do lub DW wiersz wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="d9f7d-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="d9f7d-107">Jawnie dodać użytkowników do do lub DW linii, jeśli nie można zmienić widoczności członkostwa grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d9f7d-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="d9f7d-108">Aby wyświetlić więcej szczegółów można znaleźć [HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)nieuprawnione do /_vti_bin/client.svc/sp.utilities.utility.SendEmail.</span><span class="sxs-lookup"><span data-stu-id="d9f7d-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  