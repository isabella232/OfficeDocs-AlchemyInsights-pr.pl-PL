---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688812"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="fd324-102">Odmowa dostępu podczas wyświetlania przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="fd324-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="fd324-103">Przepływy pracy programu SharePoint 2013, które próbują wysłać wiadomość e-mail do grupy programu SharePoint, mogą zakończyć się niepowodzeniem z komunikatem o błędzie "odmowa dostępu", jeśli członkostwo grupy programu SharePoint nie jest ustawione na wartość Wszyscy.</span><span class="sxs-lookup"><span data-stu-id="fd324-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="fd324-104">**Aby rozwiązać ten problem, wykonaj następujące czynności:**</span><span class="sxs-lookup"><span data-stu-id="fd324-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="fd324-105">Zezwól wszystkim na wyświetlanie członków grupy programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fd324-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="fd324-106">Usuń grupę programu SharePoint z wiersza do lub DW w wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="fd324-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="fd324-107">Jeśli nie można zmienić widoczności członkostwa w grupie programu SharePoint, należy jawnie dodać użytkowników do wiersza do lub DW.</span><span class="sxs-lookup"><span data-stu-id="fd324-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="fd324-108">Aby wyświetlić więcej szczegółów, zapoznaj się z informacjami o [protokole HTTP nieautoryzowanym do/_vti_bin/Client.svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fd324-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  